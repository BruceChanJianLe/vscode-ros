# vscode ROS

Use the configuration below for your vscode. ROS extension may not configure your vscode intellisense correctly. Hence, one may use the preconfigured file in this repository for intellisense autocomplete.

```json
{
    "configurations": [
        {
            "name": "ROS",
            "includePath": [
                "${workspaceFolder}/**",
                "/opt/ros/melodic/include/**",
                "${workspaceFolder}/include",
                "${workspaceFolder}/../../devel/include"
            ],
            "defines": [],
            "compilerPath": "/usr/bin/gcc",
            "cStandard": "c11",
            "cppStandard": "c++17",
            "intelliSenseMode": "clang-x64"
        }
    ],
    "version": 4
}
```

## intelliSenseMode Choice

Choices that have been verified to be working are `clang-64` and `gcc-x64`.

## settings.json

```json
{
    "python.autoComplete.extraPaths": [
        "/home/chanjl/test_ws/devel/lib/python2.7/dist-packages",
        "/home/chanjl/isera2_prep_box/isera2/devel/lib/python2.7/dist-packages",
        "/home/chanjl/isera2_prep_box/isera2_pack_pba/devel/lib/python2.7/dist-packages",
        "/home/chanjl/isera2_prep_box/vision_ws/devel/lib/python2.7/dist-packages",
        "/opt/ros/melodic/lib/python2.7/dist-packages"
    ],
    "c-cpp-flylint.clang.includePaths": [
        // It will be better to not include the ROS headers
        "/opt/ros/melodic/include/",
        "${workspaceFolder}/include/",
        "${workspaceFolder}/../../devel/include/",
    ],
    "c-cpp-flylint.cppcheck.includePaths": [
        // It will be better to not include the ROS headers
        "/opt/ros/melodic/include/",
        "${workspaceFolder}/include/",
        "${workspaceFolder}/../../devel/include/",
    ]
}
```
