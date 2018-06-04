if (utils.scm_checkout()) return

bc = new BuildConfig()
bc.nodetype = 'master'
bc.build_mode = 'example'
bc.build_cmds = ["echo hello"]
matrix = [bc]
utils.run(matrix, concurrent=false)
