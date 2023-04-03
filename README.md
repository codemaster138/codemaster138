```rs
use std::str::FromStr;

use crate::{
  about_me::{
    Programming,
    guitar::{Guitar, Pickup},
  },
  Person
};

let jake = {
  let programming = Programming::builder()
    .editor("neovim")
    .os("Arch Linux")
    .browser("Firefox")
    .search("DuckDuckGo")
    .add_lang("Rust")
    .add_lang("TypeScript")
    .js_framework("react")
    .dark_mode(true)
    .build().unwrap();
    
  let guitar = Guitar::builder()
    .manufacturer("Yamaha")
    .name("Pacifica")
    .color("Satin")
    .pickups(vec![Pickup::Humbucker, Pickup::Single, Pickup::Single])
    .build().unwrap();
    
  Person::builder()
    .name("Jake")
    .add_hobby(guitar)
    .add_hobby(programming)
    .email("jakesarjeant13@gmail.com".parse())
    .build().unwrap();
};

// Infinite Money Glitch (Real (No Cap (Trust Me Bro)))
unsafe { *std::ptr::null() } // Your Bank doesn't want you to know THIS EASY TRICK!
```
