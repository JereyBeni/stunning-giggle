# Starlite RE

Reverse engineering, asset research, and modding toolkit for My Talking Tom 2.

Starlite RE is a community-driven research project focused on understanding Outfit7's proprietary Starlite Engine and the resource formats used by My Talking Tom 2.

The goal is to investigate the engine's native code, document its internal architecture, understand its asset containers, and eventually develop free tools for inspecting, extracting, and modifying game resources.

«This project is currently in the research and development stage.»

🎯 Project Goals

- Reverse engineer the native Starlite Engine.
- Investigate the Raven animation system.
- Understand the "Common::Animation" framework.
- Document proprietary resource formats.
- Build custom asset inspection and extraction tools.
- Explore mesh, texture, material, skeleton, and animation resources.
- Develop a community-driven modding toolkit.

🔬 Research Targets

Native Engine

File| Purpose
"libapp.so"| Native ARM engine and game code
".text"| Executable functions
".rodata"| Strings, constants, and class references
".data"| Initialized global data
".bss"| Zero-initialized global data

Game Resources

File| Research objective
"root.assets"| Asset container and resource serialization
"root.project"| Project structure and resource references
"symbol_arm.assets"| Symbol resources and platform-specific data

The exact structures and contents of these files are still being investigated.

🧰 Tools

The project may use the following tools:

- "REA" (https://github.com/morluto/rea) - Agent-assisted reverse engineering.
- "Ghidra" (https://github.com/NationalSecurityAgency/ghidra) - Native binary analysis and decompilation.
- "Python" (https://www.python.org/) - Custom parsers and extraction utilities.
- "Blender" (https://www.blender.org/) - Inspection of supported 3D assets.
- "Git" (https://git-scm.com/) - Version control and collaboration.

🗺️ Roadmap

- [ ] Analyze the "libapp.so" ELF structure.
- [ ] Identify Starlite classes and native functions.
- [ ] Investigate Raven timelines and animation tracks.
- [ ] Investigate "Common::Animation".
- [ ] Analyze the "root.assets" header.
- [ ] Map resource tables and offsets.
- [ ] Investigate "root.project" serialization.
- [ ] Analyze "symbol_arm.assets".
- [ ] Develop a resource listing tool.
- [ ] Develop asset extraction utilities.
- [ ] Investigate resource replacement.
- [ ] Build the Starlite ModKit.

🏗️ Planned Architecture

Starlite-RE/
├── research/
│   ├── engine/
│   ├── raven/
│   ├── animation/
│   └── formats/
├── tools/
│   ├── asset-inspector/
│   ├── asset-extractor/
│   └── starlite-parser/
├── samples/
├── documentation/
└── README.md

This is a proposed structure, not a list of completed components.

📦 Modding Vision

The long-term goal is to make it possible to investigate and create custom resources for My Talking Tom 2.

Potential areas include:

- Custom textures.
- Furniture and room assets.
- Character resources.
- Animation resources.
- Toy and object resources.
- UI resources.

Actual support depends on discovering the relevant formats and engine requirements.

⚠️ Disclaimer

This is an independent, unofficial research project.

My Talking Tom 2, Starlite, and related assets and trademarks belong to their respective owners, including Outfit7.

This project is not affiliated with, endorsed by, or sponsored by Outfit7.

Do not distribute copyrighted game files or extracted assets without authorization. Use legally obtained files and respect applicable intellectual property rights.

💜 Contributing

Research, documentation, reproducible experiments, format discoveries, and improvements to the tooling are welcome.

Please distinguish confirmed findings from hypotheses when documenting discoveries.

---

Starlite RE
Understand the engine. Decode the resources. Explore the possibilities.
