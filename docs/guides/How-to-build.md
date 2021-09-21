## Prerequisites

1. Git
2. JDK 11

## Building from GitHub
1. Clone the project.

    If you want to build a release from source codes, set a `tag name` by using `git clone -b [tag_name] ...` while cloning.
    
    ```bash
    git clone --recurse-submodules https://github.com/sourceplusplus/live-platform
    cd live-platform/
    
    OR
    
    git clone https://github.com/sourceplusplus/live-platform
    cd live-platform/
    git submodule init
    git submodule update
    ```
   
1. Run `./gradlew shadowJar nativeImage makeDist -Dbuild.profile=full`
1. All packages are in `/dist`