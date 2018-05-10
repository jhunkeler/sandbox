if (utils.scm_checkout()) return

bc = BuildConfig()
bc.nodetype = ''
bc.build_mode = 'sandbox'
bc.build_cmds = [
    "echo hello world > hello.txt",
    "echo word hello > world.test",
]
bc.data_upload = [
    'generic-local/sandbox': [
        '': ['*.txt', '*.test']
    ],
]

utils.run(bc)

