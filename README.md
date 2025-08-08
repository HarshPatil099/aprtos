# 🏅 CommunityBadges Module

A simple Move smart contract for the Aptos blockchain that allows assigning and checking **user badges**, like "Top Contributor".

---

## 📦 Module Name
```move
MyModule::CommunityBadges
```

---

## 📘 Features

- ✅ Assign a badge to a user  
- ✅ Check if a user has a badge  

---

## 📄 Structs

### `Badge`
Represents a badge assigned to a user.

```move
struct Badge has key, store {
    name: string::String
}
```

---

## 🛠️ Functions

### `assign_badge(user: &signer, badge_name: string::String)`
Assigns a new badge to the given user.

### `has_badge(user: address): bool`
Checks if the given user address already has a badge.

---

## 🧪 Example Usage (CLI)

```sh
# Assign a badge
aptos move run --function-id MyModule::CommunityBadges::assign_badge --args <badge_name>

# Check if a user has a badge
aptos move run --function-id MyModule::CommunityBadges::has_badge --args <user_address>
```

> ⚠️ Replace `MyModule` with your actual account address if deploying on chain.

---

## 📁 File Structure

```
/sources
  └── CommunityBadges.move
Move.toml
README.md
```

---

## ✅ Requirements

- [Aptos CLI](https://aptos.dev/tools/aptos-cli/)
- Rust & Cargo

---

## 🧑‍💻 Author

Created by harsh – feel free to contribute!

---

## 📜 License

MIT License
