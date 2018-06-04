if (utils.scm_checkout()) return

def body = """
{
    "glossary": {
        "title": "example glossary",
		"GlossDiv": {
            "title": "S",
			"GlossList": {
                "GlossEntry": {
                    "ID": "SGML",
					"SortAs": "SGML",
					"GlossTerm": "Standard Generalized Markup Language",
					"Acronym": "SGML",
					"Abbrev": "ISO 8879:1986",
					"GlossDef": {
                        "para": "A meta-markup language, used to create markup languages such as DocBook.",
						"GlossSeeAlso": ["GML", "XML"]
                    },
					"GlossSee": "markup"
                }
            }
        }
    }
}
"""
dc = new DataConfig()
dc.insert('PLZWORK', body)
bc = new BuildConfig()
bc.nodetype = 'linux'
bc.build_mode = 'example'
bc.build_cmds = ["echo hello"]
//bc.test_cmds = [
//    'echo [{"test2":"alive2"}] > test2.json',
//]
bc.test_artifacts = [dc]
matrix = [bc]
utils.run(matrix)
