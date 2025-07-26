# Soundness CLI - PROOF Tutorial

## NOTES:

1. This tutorial is for **anyone having trouble doing the PROOF via CLI**.
2. It is for those who **have the KEY’s secret phrase (Mnemonic)**.

    2.1 The **secret phrase (Mnemonic)** was generated when you created the key and contains **12, 16, 18, or 24 words**.

3. If you **don’t have the Mnemonic**, you will need to **generate a new key**. This tutorial will be updated based on demand.

---

## CLI SETUP:

1. **Create a repository** on your GitHub by clicking **"New"**.

   ![Step 1](https://github.com/user-attachments/assets/c421acf0-12fb-4eb1-b705-beaec5f96219)

1.1 **Configure the repository like this** and click **"Create Repository"**:

   ![Step 1.1](https://github.com/user-attachments/assets/f0315376-310d-4a0c-ad89-14ed07370fb4)

2. Go to the **four dots at the top** and click on **"Codespaces"**:

   ![Step 2](https://github.com/user-attachments/assets/2c652e75-e380-49e3-9193-b47d394d3672)

2.1 Click **"New Codespace"** and configure it like this:

   ![Step 2.1](https://github.com/user-attachments/assets/5441952b-1e22-4b19-8e94-c87c5ee7ea81)

2.2 Then click **"Create Codespace"**

3. After Codespace loads, you will see this screen:

   ![Step 3](https://github.com/user-attachments/assets/887fdccf-48be-44d4-ab1a-cdf3ccc42d6a)

---

## SETTING UP SOUNDNESS LAYER

> ⚠️ Paste the commands **one by one**. Wait for one to finish before pasting the next.

Open the terminal like this:

![Terminal View](https://github.com/user-attachments/assets/6b07b29b-bf96-4c61-bc42-6702b5059706)

### Run the following commands:

1.
```bash
sudo apt update && sudo apt upgrade -y
```

2.
```bash
curl -sSL https://raw.githubusercontent.com/soundnesslabs/soundness-layer/main/soundnessup/install | bash
```

3.
```bash
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs/ | sh
```

4.
```bash
source ~/.bashrc
```

5.
```bash
soundnessup install
```

6.
```bash
soundnessup update
```

---

## IMPORTING YOUR SECRET PHRASE (Mnemonic)

```bash
soundness-cli import-key --name my-key --mnemonic "YOUR SECRET PHRASE HERE"
```

### Notes:

- In `--name my-key`, use the name you saved your key as. If you didn’t, just leave it as `my-key`.
- If successful, it will ask you to enter your password twice.
- Paste your secret phrase (12, 16, 18, or 24 words) inside the quotes.

---

## RUNNING THE PROOF

> ✅ **If you completed the game and got a message from the bot like this:**

![Bot Message](https://github.com/user-attachments/assets/6aa2e2c7-e0f3-44fb-9994-158754de5422)

1. Copy the command and replace `"your-key-name"` with `my-key`, like this:

   ![Key Replacement](https://github.com/user-attachments/assets/399c7cd8-56b4-4d36-9a6b-23fb12827597)

2. Paste the command in the terminal and press Enter. It will load the **Walrus** and **Sui** APIs and ask for your password.

3. If all goes well, you’ll see a response like this:

   ![Success Response](https://github.com/user-attachments/assets/455aea47-9ede-4393-8240-637ae557a93e)

---

Once that appears, **your proof is successfully completed** ✅
