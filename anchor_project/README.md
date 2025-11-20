# Blog Program

An **Anchor** program for the Solana blockchain that allows users to create and manage decentralized blogs. This program supports initializing a blog and adding posts. Made by a begginer Solana Dev.


## Introduction

This Solana program enables users to:
1. Initialize a decentralized blog.
2. Add posts to the blog, each linked to the previous one, forming a chain of posts.

### Key Features
- **Authority Management**: Each blog is owned by an authority.
- **Post Linking**: Every new post is linked to the previous one, allowing post history tracking.
- **Dynamic Storage**: Post accounts are dynamically sized based on the length of the title and content.

---

## Program Structure

### Core Instructions

1. **`initialize`**: Sets up a new blog.
2. **`create_post`**: Adds a new post to the blog.


### Instruction Descriptions
**`initialize`**: Initializes a new blog account.

## Parameters
**Authority**: The signer who owns the blog.

## Account Context
**authority**: The signer of the transaction.
**blog**: The newly initialized blog account.
**system_program**: Solana's system program for account creation.

### Instruction Descriptions
**`create_post`**: Adds a new post to an existing blog.

## Parameters
**title**: Title of the post.
**content**: Content of the post.

## Account Context
**authority**: The signer of the transaction.
**blog**: The blog account to which the post is being added.
**post**: The newly created post account.
**system_program**: Solana's system program for account creation.