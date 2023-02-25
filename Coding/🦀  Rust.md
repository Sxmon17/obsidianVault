#Coding #Rust 

## Useful Snippets
Snippets for Rust and its Frameworks

### Tokio.rs
##### Client
```Rust
//connect to the server with tokio  
let mut stream = tokio::net::TcpStream::connect(CHAT_SERVER).await.unwrap();  
  
//create a channel to send messages to the server  
let (mut tx, mut rx) = tokio::io::split(stream);
```

##### Client
