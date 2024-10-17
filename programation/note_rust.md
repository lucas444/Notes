# Note rust 

## lien 

[rustbook](https://jimskapt.github.io/rust-book-fr/)

## 1er code :

```rs
fn main(){
    println!("Hello World !");
}
```

## Variable
let a = 15;
let mute b = 12;



## Fonction
fn saluer(){
	println!("Yo");
}


## Cargo


Compilateur de rust

`cargo --version`
> Pour voir la version

`cargo new hello\_word`
> Créé un projet rust 
le fichier *Cargo.toml* donne les information sur le projet et un dossuer *src* pour acceuillieur le code

```rs
[package]
name = "hello_cargo"
version = "0.1.0"
edition = "2021"

[dependencies]
```

`cargo build #compile le projet`
`cargo run #compile puis execute`
`cargo chek #compile rapidement le programe pour verifier`
