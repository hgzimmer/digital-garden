# Setup

## obsidian-export

Source: [GitHub - zoni/obsidian-export: Rust library and CLI to export an Obsidian vault to regular Markdown](https://github.com/zoni/obsidian-export)
I decided to install the binary via cargo-binstall as I don't have rust and the corresponding toolchain installed on my laptop at the moment.

### First
``` bash
brew install cargo-binstall
```
### Then
``` bash
cargo-binstall obsidian-export
```
Output
```bash

 INFO **resolve**: Resolving package: 'obsidian-export'

 WARN The package obsidian-export v23.12.0 (aarch64-apple-darwin) has been downloaded from github.com

 INFO This will install the following binaries:

 INFO   - obsidian-export => /Users/heiko/.cargo/bin/obsidian-export

Do you wish to continue? [yes]/no

? 

 INFO Installing binaries...

 INFO Done in 18.621516041s
 ```
### Result
Please note the path it was installed in ```/Users/heiko/.cargo/bin/obsidian-export```

## quartz
Clone the directory and then follow [quartz/docs/index.md at v4 · jackyzha0/quartz · GitHub](https://github.com/jackyzha0/quartz/blob/v4/docs/index.md)

npm i
npx quartz create
