python_binary(
  name = 'thermos_executor',
  source = 'thermos_executor_main.py',
  entry_point = 'apache.aurora.executor.bin.thermos_executor_main:proxy_main',
  ignore_errors = True,
  always_write_cache = True,
  dependencies = [
    pants('aurora/twitterdeps/src/python/twitter/common/app'),
    pants('aurora/twitterdeps/src/python/twitter/common/log'),
    pants('aurora/twitterdeps/src/python/twitter/common/metrics'),
    pants('src/main/python/apache/aurora/executor/common:executor_timeout'),
    pants('src/main/python/apache/aurora/executor/common:health_checker'),
    pants('src/main/python/apache/aurora/executor/common:sandbox'),
    pants('src/main/python/apache/aurora/executor:executor_detector'),
    pants('src/main/python/apache/aurora/executor:executor_vars'),
    pants('src/main/python/apache/aurora/executor:thermos_executor'),
    pants('src/main/python/apache/aurora/executor:thermos_task_runner'),
  ]
)

python_binary(
  name = 'gc_executor',
  source = 'gc_executor_main.py',
  entry_point = 'apache.aurora.executor.bin.gc_executor_main:proxy_main',
  ignore_errors = True,
  always_write_cache = True,
  dependencies = [
    pants('aurora/twitterdeps/src/python/twitter/common/app'),
    pants('aurora/twitterdeps/src/python/twitter/common/log'),
    pants('aurora/twitterdeps/src/python/twitter/common/metrics'),
    pants('src/main/python/apache/thermos/common:path'),
    pants('src/main/python/apache/aurora/executor:executor_detector'),
    pants('src/main/python/apache/aurora/executor:executor_vars'),
    pants('src/main/python/apache/aurora/executor:gc_executor'),
  ]
)

python_binary(
  name = 'thermos_runner',
  source = 'thermos_runner_main.py',
  entry_point = 'apache.aurora.executor.bin.thermos_runner_main:proxy_main',
  dependencies = [
    pants('aurora/twitterdeps/src/python/twitter/common/app'),
    pants('aurora/twitterdeps/src/python/twitter/common/log'),
    pants('src/main/python/apache/aurora/executor:thermos_runner'),
  ],
)
