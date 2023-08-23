btsniffer - um farejador que fareja torrents da rede BitTorrent
========================================

## Introdução

Refatorado

> *Aprimoramento:* Também peca na rede BitTorrent, mas armazena apenas torrents que atingem suas palavras-chave.

## Compilando

> Certifique-se de ter golang instalado em seu ambiente de sistema
```bash
./build.sh
```

## Uso

```
$ ./btsniffer -h

Uso:
   torsniff [bandeiras]

Bandeiras:
   -k, --kwfile string o arquivo de palavras-chave (padrão ./keywords.txt; dividido por linha)
   -o, --database string o banco de dados de saída, todos os torrents serão salvos nesse arquivo (padrão ./torrentdata.db)
   -a, --addr string escuta em determinado endereço (padrão todos, ipv4 e ipv6)
   -d, --dir string o diretório para armazenar os torrents (padrão "$HOME/torrents")
   -f, --friends int max demônios para fazer por segundo (padrão 500)
   -e, --peers int max peers para conectar para baixar torrents (padrão 400)
   -p, --port uint16 escuta em determinada porta (padrão 6881)
   -t, --timeout duração tempo máximo permitido para download de torrents (padrão 10s)
   -h, --help ajuda para torsniff
   -v, --verbose executado em modo detalhado (padrão verdadeiro)
```

## Começo rápido
Use sinalizadores padrão:

`./btsniffer`


## Referências de Protocolos
- [Protocolo DHT](http://www.bittorrent.org/beps/bep_0005.html)
- [A especificação do protocolo BitTorrent](http://www.bittorrent.org/beps/bep_0003.html)
- [Protocolo de extensão BitTorrent](http://www.bittorrent.org/beps/bep_0010.html)
- [Extensão para pares enviarem arquivos de metadados](http://www.bittorrent.org/beps/bep_0009.html)# BitNetWork
