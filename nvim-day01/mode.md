# Mode in Neovim

There's 4 mode in Nvim (Neovim):

1. Normal (For reading and navigating)

Press escape or ctrl [ to enter this mode, mainly used for navigating and operator.

2. Insert (For coding/inserting character)

Press i, a, o or their capital version to enter this mode:
i for inserting behind the cursor.
a for inserting after cursor.
o for inserting new line below and enter insert mode.

There's capital version of these button, (I, A, O):
I for inserting at the start of line.
A for inserting at the end of line.
O for inserting new line above and enter insert mode on your current line.

3. Visual (For mass editing)

Press v, V, ctrl v to enter this mode:
v for selecting character by character.
V for selecting 1 line.
ctrl v for selecting block of code (Rectangular block).

4. Command (For using command in Nvim)

Press : (Colon) to enter this mode.
Press / (Slash) to enter search forward.
Press ? (Question mark) to enter search backward

AI Version

# Mode — Day 01

- Normal: mode default, navigasi dan operator. Kembali dengan `Esc`.
- Insert: mengetik teks. Masuk dengan `i`, `a`, `o`, `O`.
  - `i` — insert sebelum kursor
  - `a` — insert setelah kursor
  - `o` — baris baru di bawah, lalu insert
  - `O` — baris baru di atas, lalu insert
- Visual: seleksi. Masuk dengan `v`, `V`, `Ctrl+v`.
- Command-line: perintah dengan `:`.

Jika bingung sedang di mode apa: tekan `Esc`, lalu coba `j` atau `k`.
