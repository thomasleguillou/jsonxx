Import('env')
localEnv = env.Clone()

sources = [
'jsonxx.cc',
]

jsonxx = localEnv.Library('jsonxx', sources )
localEnv.Prepend(LIBS=jsonxx)

testList =  [
'jsonxx_test.cc',
]

localEnv.Program('jssoxx_test',testList, CXXFLAGS='-Wall -W -Wextra')

Return('jsonxx')