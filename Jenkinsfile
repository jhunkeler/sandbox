if (utils.scm_checkout()) return

dc = new DataConfig()
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
