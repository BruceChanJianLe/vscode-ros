# vsocde ROS

Use the configuration below for your vscode. ROS extension may not configurate your vscode intellisense correctly. Hence, one may use the preconfigurate file in this repository.

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