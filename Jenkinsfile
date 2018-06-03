if (utils.scm_checkout()) return

data_configs = []
dc = new DataConfig()
dc.insert('test', '{"test":"alive"}')

data_configs += dc

bc = new BuildConfig()
bc.nodetype = 'master'
bc.build_mode = 'sandbox'
bc.build_cmds = ["echo hello"]
//bc.build_cmds = [
//    "echo {\"test\":\"alive2\"} > alive.json"
//]
bc.test_artifacts = data_configs

utils.run(bc)

