* 重复执行的时候，不再重复执行portable-msvc.py
* $env:DisableRegistryUse="true"放在原来位置的化，funchook编译会失败，所以挪到下面
* zlib需要编译，否则会提示zlibstatic.lib找不到
* ep_setup编译的时候因为有clean，导致生成的ep_setup_files.zip里文件缺失，所以需要第二次不加clean的编译，才能创建完整的ep_setup_files.zip
* 修正一些路径错误
