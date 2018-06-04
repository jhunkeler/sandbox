if (utils.scm_checkout()) return

dc = new DataConfig()
dc.insert('test', '{"test":"testing"}')
bc = new BuildConfig()
bc.nodetype = 'linux'
bc.build_mode = 'example'
bc.build_cmds = ["echo hello"]
bc.test_cmds = ["echo '{\"test\":\"alive\"}' > test.json"]
bc.test_artifacts = [dc]
matrix = [bc]
utils.run(matrix)
