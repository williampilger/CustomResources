# Assinatura de E-mail IFRS (design pessoal)

*Esta assinatura de e-mail **não** segue nenhum padrão do IFRS.


Criação dos logos `.png`, eu uso de referência as logos em SVG, mas para fins de utilização real, só é possível usar as logos em PNG.

Elas foram geradas usando o ImageMagick:

> magick .\facebook.svg -resize 50x50! .\facebook.png

Ou, automatizar isso:

* Windows:
  * ```ps1
    Get-ChildItem -Filter *.svg | ForEach-Object {
        magick $_.FullName -resize 50x50! -background none ($_.BaseName + ".png")
    }
    ```
* Linux:
  * ```sh
    for file in *.svg; do
        magick "$file" -resize 50x50! -background none "${file%.svg}.png"
    done
    ```


## Sobre

A logo foi obtida [do site oficial do IFRS](https://ifrs.edu.br/institucional/comunicacao/materiais-para-download/#gallery-2) em *2025/03/11 10:53:10*.