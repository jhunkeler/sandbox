if (utils.scm_checkout()) return

dc = new DataConfig()
dc.server_id = 'artifactory'
dc.match_prefix = "(.*)_result"

bc = new BuildConfig()
bc.nodetype = 'linux'
bc.build_mode = 'example'
bc.build_cmds = ["echo hello"]
bc.test_configs = [dc]

matrix = [bc]
utils.run(matrix)
