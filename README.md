# FiscalBox – versões

Este repositório contém **somente os instaladores publicados** do FiscalBox (aba *Releases*).
O código-fonte é privado.

Cada versão traz:

- `FiscalBox-<versão>.msi` – instalador para Windows (Java embutido, instalação por usuário, sem administrador);
- `atualizacao.properties` – descrição da versão (número, arquivo, SHA-256, tamanho, novidades);
- `atualizacao.properties.assinatura` – assinatura Ed25519 da descrição.

O FiscalBox só instala uma atualização se a assinatura conferir com a chave pública embutida no
programa e se o SHA-256 do instalador baixado for igual ao da descrição assinada.
