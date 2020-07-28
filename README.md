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
                "${workspaceFolder}/include"
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
