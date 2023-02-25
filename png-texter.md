#Rust #Coding #ReadMeSamples 
# png-texter
A CLI tool to hide encrypted messages in a .png file written in [[Rust]]
</br>

## 💎 Features
- [x] Png chunk editor
- [x] Url as input source
- [x] Custom chunk type (password to decode)
- [x] Rich and colorful Cli
- [ ] Gui
- [ ] Web Interface
- [ ] Chunk Viewer
- [ ] Interface to send pngs over network

## 👾 Usage 
<details>
<summary> 🐧 Linux </summary>
<p>

```bash
   ~/png-texter help
```

</p>
</details>
<details>
<summary> 🪟 Windows </summary>
<p>

```bash
   C:\png-texter.exe help
```

</p>
</details>

</br>

## ~/png-texter help
```
A simple png chunk message encoder/decoder

Usage: png-texter [OPTIONS] [COMMAND]

Commands:
  encode  encode the png with a secret message
  decode  decode the png to get the secret message
  remove  remove the chunk from the png
  help    Print this message or the help of the given subcommand(s)

Options:
  -c, --chunk-type <CHUNK_TYPE>  Sets the chunk type to use
  -h, --help                     Print help
  -V, --version                  Print version
```

## ~/png-texter help encode


```
encode the png with a secret message

Usage: png-texter encode [OPTIONS] [FILE] [SECRET_MSG]

Arguments:
  [FILE]        Png to encode
  [SECRET_MSG]  Secret message to encode within the png

Options:
  -o, --output <output>  Output png
  -u, --url <url>        source from url
  -h, --help             Print help

```

## 🔬 Examples 

### Path Source

![image](https://user-images.githubusercontent.com/65186979/218119450-3970c6d7-b7ac-4908-be7b-6490e560ce04.png)

#### Encode
``` bash
~/png-texter -c "rust" encode -o "png_tests/encoded.png"  png_tests/example.png "Hello User!"
```
#### Decode
``` bash
~/png-texter -c "rust" decode png_tests/encoded.png
```
#### Remove
``` bash
~/png-texter -c "rust" remove png_tests/encoded.png
```
</br>

### Url Source

![image](https://user-images.githubusercontent.com/65186979/219093918-c4555974-167a-4a0a-bfce-36fd38839b3e.png)

#### Encode from url
``` bash
~/png-texter encode -u "https://www.fnordware.com/superpng/pnggrad8rgb.png" png_tests/url_encoded.png "Hello User :)"
```      
</br>

## 📝 [[License]]

Copyright © 2023 [Simon Guglberger](https://github.com/sxmon17).</br>
This project is [MIT](https://github.com/Sxmon17/png-texter/blob/main/LICENSE.md) licensed.


##### If you find a bug or have an idea for a new feature, please open an issue or submit a pull request.