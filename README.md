# lukewarm20-offline-encryption-computation

This contains a raspberry pi and a camera

Taking the raspberry pi and attaching a camera, keeping the keys of your messages on it instead of the device you are communicating on will allow you to decrypt your messages on the raspberry pi instead of the device you are using to communicate, this means that you will have an air gapped machine that you can encrypt your mesages on, then port over to any machine to go out to the internet. Meaning that the original message is no longer anything anyone can read. Even if the raspberry pi/air gapped machine is compromised, it won't make a difference. As long as you keep this machine safe, and away from anyone being able to tamper with it, you have a method of being able to communicate without anyone in the middle or on the online computer knowing.

The setup is simple, you will need qrencode, gnupg, raspberry pi, and camera attached to said pi.

Write the message out on the pi, encrypt using gnupg with the proper keys for either public key or private key cryptography. Encode the data and write to a picture using qrencode, then turn the display of the pi on. Setup the same method on the device online, using this method, you can transfer the encrypted information to the other computer without it even knowing what the message was originally. Same goes the other way around.
