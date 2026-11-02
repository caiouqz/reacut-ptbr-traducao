ReaCut em português brasileiro (PT-BR)

Tradução não oficial da interface do **ReaCut 0.6.0 para Windows**. Ela traduz os principais menus, abas, controles e mensagens. Alguns nomes de efeitos, recursos e mensagens ainda podem aparecer em inglês.

Este pacote é para o ReaCut, não para o editor CapCut. Não inclui o instalador do ReaCut nem o FFmpeg. É necessário já ter o ReaCut instalado. Esta tradução foi testada abrindo uma cópia isolada do programa; a importação, edição e exportação não foram testadas de ponta a ponta.

## Projeto e créditos

Esta tradução é uma adaptação não oficial para português brasileiro da versão Windows do [ReaCut de justelson/rea-capcut](https://github.com/justelson/rea-capcut), que é um fork do [projeto original de Xiangyu-CAS](https://github.com/Xiangyu-CAS/rea-capcut). O ReaCut é um editor independente; esta tradução não representa uma versão oficial do projeto.

O código original usa a licença MIT. A licença e os avisos de terceiros fornecidos pelo repositório estão incluídos neste pacote.

## Instalação

1. Confira se o programa instalado é o ReaCut **0.6.0**. Outras versões podem ser incompatíveis.
2. Salve seus projetos e feche o ReaCut completamente.
3. Abra a pasta de instalação do programa e entre em `resources`. No caminho padrão, ela fica em:

   `C:\Users\SEU_USUARIO\AppData\Local\Programs\reacut\resources`

4. Dentro de `resources`, renomeie o arquivo original `app.asar` para `app.asar.original`. Se já existir um arquivo com esse nome, guarde o original em outro local seguro; não o substitua.
5. Copie o `app.asar` deste pacote para a pasta `resources`.
6. Abra o ReaCut. Para voltar ao idioma original, feche o programa, remova o `app.asar` traduzido e renomeie a cópia de segurança `app.asar.original` para `app.asar`.

O arquivo original de referência da versão testada tem SHA-256 `d7dd1e28218cf9dfdfaaf3417d565f09759f71636a8d2344293770f457cf4cb6`. Se for diferente, a instalação pode ser outra versão: não substitua o arquivo sem verificar a compatibilidade.

No PowerShell, é possível conferir o arquivo antes de renomeá-lo:

```powershell
Get-FileHash -Algorithm SHA256 "$env:LOCALAPPDATA\Programs\reacut\resources\app.asar"
```

Uma atualização do ReaCut pode substituir a tradução ou torná-la incompatível. Se ocorrer algum problema, restaure o backup.

## Importação de vídeos e FFmpeg

Se aparecer uma mensagem dizendo que o `ffprobe` não foi encontrado, instale uma distribuição Windows confiável do FFmpeg que contenha **ffmpeg.exe** e **ffprobe.exe**. A [página de downloads do FFmpeg](https://ffmpeg.org/download.html) indica fornecedores de compilações para Windows. Extraia os arquivos e, nas configurações do ReaCut, selecione os dois executáveis. Reinicie o aplicativo se necessário.

A tradução não inclui arquivos de vídeo nem modifica seus projetos. O programa, seus componentes e marcas pertencem aos respectivos autores. Confira as licenças e autorizações aplicáveis antes de redistribuir este pacote, pois ele contém arquivos do aplicativo.
