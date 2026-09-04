# zComercial Desktop

Distribuição da aplicação de secretária do **zComercial** — facturação
electrónica certificada pela AGT, em Angola.

Este repositório **não contém código-fonte**. Existe para alojar:

- os instaladores de cada versão, em [Releases](../../releases);
- o `appcast.xml`, que a aplicação instalada consulta para saber se há versão
  mais recente;
- as notas de cada versão.

## Descarregar

A versão mais recente está sempre em **[Releases](../../releases/latest)**.

Requisitos: Windows 10 ou 11, 64 bits. A instalação é por utilizador — não
pede palavra-passe de administrador.

## Verificar o que descarregou

Cada versão traz um `SHA256SUMS.txt`. Para conferir, no PowerShell:

```powershell
Get-FileHash .\zComercial-Windows-<versão>-Setup.exe -Algorithm SHA256
```

O valor tem de coincidir com o do ficheiro.

## O aviso do Windows

Ao abrir o instalador, o Windows mostra **«O Windows protegeu o seu PC»**.
É esperado: o instalador ainda não é assinado com um certificado Authenticode.
Carregue em *Mais informações* e depois em *Executar mesmo assim*. Confira o
SHA-256 acima se quiser certificar-se de que o ficheiro é o nosso.

## Suporte

[zcomercial.com](https://zcomercial.com)
