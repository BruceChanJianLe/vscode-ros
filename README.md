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
