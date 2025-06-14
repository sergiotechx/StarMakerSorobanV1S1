**Fundamentos de RUST 🦀**

Todo el código lo correremos en el playground de Rust, no necesitamos instalar absolutamente nada

[**https://play.rust-lang.org/**](https://play.rust-lang.org/)

Primeros pasos en Rust

**Pimer hola mundo:**

```plaintext
fn main() {
    println!("Hello, world!");
}
```

**Declaración de Variables**

```plaintext
fn main(){
   // Variable inmutable (por defecto)
   let nombre = "Juan";
   println!("nombre {}",nombre);

   // Variable mutable
   let mut edad = 25;
   println!("edad: {}",edad);
   edad = 26; // ✅ Permitido
   println!("nueva edad: {}",edad);

   // Constante
   const PI: f64 = 3.14159;
   println!("PI: {}",PI);
}
```

**Tipos Básicos**

```plaintext
fn main(){
  // Números enteros
  let numero: i32 = 42;
  let grande: u64 = 1000000;

  // Números decimales
  let precio: f64 = 19.99;

  // Texto
  let mensaje: String = String::from("Hola Soroban");
  let letra: char = 'A';

  // Booleano
  let activo: bool = true;
  println!("numero: {} grande: {} precio: {}",numero,grande,precio);
  println!("mensaje: {} letra: {} activo: {}",mensaje,letra,activo);
}
```

**Funciones**

```plaintext
// Función simple 
fn saludar() {
  println!("¡Hola mundo!"); 
}

// Función con parámetros 
fn sumar(a: i32, b: i32) -> i32 {
  // Sin punto y coma = return 
    a + b 
}

fn main() { 
       saludar(); 
       let resultado = sumar(5, 3); 
       println!("5 + 3 = {}", resultado);
 }
```

**If/Else**

```plaintext
fn evaluar_edad(edad: u32) {
   if edad < 13{
        println!("Eres menor de edad");
   }
   else if edad >= 13 && edad < 18{ 
             println!("Eres adolescente"); 
   } 
   else { 
         println!("Eres mayor de edad");  
   }
 }

fn main(){
  evaluar_edad(18);
}
```

**Más información de  Rust**

[https://book.rustlang-es.org](https://book.rustlang-es.org)
