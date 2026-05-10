# Site Busca Universal Pro em ISO / Arquivos de Jogos

Abra `index.html` no navegador.

Esta versão tenta:
- texto normal em vários encodings
- UTF-8, ASCII, Latin-1, Windows-1252
- UTF-16 LE/BE e UTF-32 LE/BE
- Shift-JIS, EUC-JP, GBK, Big5, EUC-KR
- tabela própria
- GZIP
- ZLIB/Deflate
- Deflate bruto
- entradas ZIP locais
- tentativa de listar arquivos em ISO 9660
- XOR 1 byte com chaves 00-FF
- NOT/inverter bits
- soma/subtração de 1 byte
- nibble swap
- texto invertido

Limitação importante:
Criptografia real sem chave não é possível descriptografar automaticamente.
Compressão própria de jogos, LZSS/LZ77 custom, arquivos com ponteiros, imagens e tabelas próprias podem precisar de extrator específico.
