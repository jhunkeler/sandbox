if (utils.scm_checkout()) return

//dc = new DataConfig()
//dc.insert('test', '{"test":"alive"}')

bc = new BuildConfig()
bc.nodetype = 'linux'
bc.build_mode = 'sandbox'
bc.build_cmds = ["echo hello"]
//bc.test_artifacts = dc

utils.run(bc, concurrent=false)

