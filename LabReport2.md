# Lab Report 2
## Part 1
### My Code
![ChatServer_Code.png](/images/LB2/ChatServerCode.png)

#### /add-message Sample 1
![CreatorMessage.png](/images/LB2/CreatorMessage.png)
* The only method called in my code that is called is `handleRequest` in the `Handler` class, which implements the interface `URLHandler`.
* The relevant argument for `handleRequest` is `url` of type `URL` which in this case is http://localhost:4020/add-message?s=It%20is%20a%20me!%20The%20creator%20of%20this%20server's%20code!&user=Bob, and the value of the field `conversation` of the class before the method is run is this point `"Sammy: Hello!"`.
* My value `conversation` got changed to `"Sammy: Hello! \n Sammy: It is a me! The creator of this server's code!"`.

#### /add-message Sample 2
![BobMessage.png](/images/LB2/BobMessage.png)
* The only method called in my code that is called is `handleRequest` in the `Handler` class, which implements the interface `URLHandler`.
* The relevant argument for `handleRequest` is `url` of type `URL` which in this case is http://localhost:4020/add-message?s=Wow!%20You%20are%20amazing!&user=Bob, and the value of the field `conversation` of the class before the method is run is this point `"Sammy: Hello! \n Sammy: It is a me! The creator of this server's code!"`.
* My value `conversation` got changed to `"Sammy: Hello! \n Sammy: It is a me! The creator of this server's code! \n Bob: Wow! You are amazing!"`.

## Part 2

* Using the ls command with the absolute path to the private key:

![lsCommandForPrivate.png](/images/LB2/lsCommandForPrivate.png)

* Using the ls command from the remote server for the absolute path to the public key:

![lsCommandForPublicFromRemote.png](/images/LB2/lsCommandForPublicFromRemote.png)

* Logging in to the remote server without a password:

![loggingInWithoutPassword.png](/images/LB2/loggingInWithoutPassword.png)

## Part 3
Something that I learned from lab that I didn't know before would be the meyjod to logging into a computer remotely. While I did know we could from lecture, I didn't know how to do so myself before lab.
