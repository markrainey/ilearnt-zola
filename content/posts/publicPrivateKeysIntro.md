+++
title="Public/Private keys introduction"
description="A very simple high level introduction to public and private keys and how they are used"
date=2023-06-30
authors = ["Mark Rainey"]
[taxonomies]
categories=["misc"]
tags=[]
+++

I recently had to try and explain to some non-technical colleagues how part of our system works. This involved giving them a very quick overview of public/private key cryptography. So I thought I would summarise it here.

<!-- more -->

Imagine a padlock that has two keyholes - one accepts a key called "Private" and the other accepts a key called "Public". If a user, Alice, locks the padlock with the private key then it can only be unlocked with the public key. Similarly, if Alice locks it with the public key it can only be unlocked with the private key.

Alice must keep her private key private - she must be the only one who has access to it. However she can give her public key to anyone.

<img src="/posts/PublicPrivateKeys.png" title="Keys" class="mid-image"></img><p></p>
So how is this useful?

# Encryption

Someone can take some data and use Alice's public key to **encrypt** (lock) it. This means that the only person who can **decrypt** (unlock) it is Alice as the only key that can unlock it is Alice's private key. So this means that someone can send Alice some data, or a message, that only she can read as she is the only one who can unlock it.

<img src="/posts/Encryption.png" title="Encryption" class="mid-image"></img>

# Signing

If we reverse the process then we can get another useful feature. If Alice takes her private key and **signs** (locks) the data she can send it to anyone. If the private key is used then the only key that can be used to unlock it is the public key. Anyone with Alice's public key can then **verify** (unlock) that the data was signed with Alice's private key. As Alice is the only person with access to the private key it means we know that Alice must have been the one to have sent the data.

<img src="/posts/Signing.png" title="Signing" class="mid-image"></img>

