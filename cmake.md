
## file format
filename: CMakeLists.txt

## command option

### pre-build

cmake -S $source_dir -B $build_dir

### build
cmake --build $build_dir --config $build_type(default is Debug, Release) -j $build_thread_num
