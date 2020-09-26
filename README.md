# vim-42header
a (better) vim header for 42 projects

![fancy header image](http://i.imgur.com/WTscMvi.png)

## forked for
42서울 카뎃들의 메일 주소가 길어서 원본 플러그인을 사용할 시 헤더가 깨지는 문제가 발생할 수 있습니다.
이를 방지하기 위해 약간의 수정을 해서 제가 빨리 사용하려고 그냥 fork했습니다.
아래 사용방법 항목에서 pbondoer 부분을 goyarn 으로 고쳐주시면 됩니다.

I'm in 42Seoul, and Seoul cadets have long mail. (mine is ...@student.42seoul.kr)
So I fixed a line about putting padding between mail and ascii art.
Thanks!

## Features
* Passes `norminette`
* Elegant trimming of long strings
* Updates filename line when changed
* Updates "Updated" line only when buffer is changed
* Works with all formats that default supports
* Binds to `F1` for easy access
* Overrides `:Stdheader` for school vim installs

Also, don't forget to set your `$USER` and `$MAIL` variables, marvin lives!
### 유저, 메일 설정 방법
```vim
" in ~/.vimrc
let g:hdr42user = 'yourlogin'
let g:hdr42mail = 'yourmail@student.42seoul.kr'
```

## Usage

### No plugin manager
Copy `42header.vim` to your `~/.vim/after/plugin/` folder. You're set!

### pathogen
```
git clone https://github.com/pbondoer/vim-42header.git --recursive && mv -v vim-42header ~/.vim/bundle/
```

### vim-plug
If you use vim-plug or any other plugin manager, simply add this line to your
plugin initialization:

```vim
Plug 'pbondoer/vim-42header'
```

## Why?
Part of the **Mexican Standoff** rush, I decided to add a few bonus features
and I now use this as my header for 42 files. On my linux setup, I have changed
the variable names in order to be able to have my own environment, but still
have a functional school environment. Feel free to add things :)!
