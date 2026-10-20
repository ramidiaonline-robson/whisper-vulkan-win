# whisper.cpp com Vulkan para Windows x64

O projeto oficial [ggml-org/whisper.cpp](https://github.com/ggml-org/whisper.cpp) não publica binários com Vulkan para Windows.
Este repositório só compila o código **oficial, sem alterações**, na tag indicada, com `-DGGML_VULKAN=ON`, e publica o zip na aba Releases.

- Estrutura do zip: pasta `Release/` com `whisper-cli.exe` e as DLLs (igual aos pacotes oficiais).
- Não exige nada além do `vulkan-1.dll` que já vem com o driver da placa de vídeo (AMD, Intel Arc, NVIDIA).
- O build roda no GitHub Actions (`.github/workflows/build.yml`), de forma auditável.
- Usado pelo instalador automático do AtaFlow AI (RA Mídia Online).
