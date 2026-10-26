# iAcode-OS · versões

Aqui ficam as **versões publicadas do iAcode-OS**: um assistente de IA self-hosted (IAs locais e na nuvem, num só lugar) que vira um sistema instalável.

> O código-fonte é privado. Este repositório só distribui as versões.

## O que tem em cada release

| Arquivo | Para quê |
|---|---|
| `manifest.txt` + `manifest.txt.sig` | A ficha da versão, assinada (Ed25519). As máquinas conferem a assinatura antes de baixar qualquer coisa. |
| `iacode-os-X-instalacao.tar.gz` | Compose, scripts e o iAcode Agent (sem código-fonte). |
| `*.tar.zst` (ou `.parteNN`) | As imagens Docker que mudaram nesta versão. |

## Atualizações automáticas

Todo iAcode-OS procura versão nova aqui a cada ~6 horas (`releases/latest/download/manifest.txt`) e mostra o aviso **"Atualização disponível"** no app.
O administrador atualiza com um clique, ou liga **"Instalar atualizações sozinho"** para atualizar de madrugada.
Se a versão nova não subir, ele volta sozinho para a anterior.
