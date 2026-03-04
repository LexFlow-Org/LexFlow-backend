# LexFlow — Backend & Bridge

Rust/Tauri backend e JavaScript bridge per l'app LexFlow.

## Struttura

```
src-tauri/
  src/
    lib.rs          # Core backend — comandi Tauri, vault, crypto, scheduler
    main.rs         # Entry point
  Cargo.toml        # Dipendenze Rust
  Cargo.lock        # Lock file
  tauri.conf.json   # Configurazione Tauri
  build.rs          # Build script
  Info.plist        # macOS metadata
  capabilities/
    default.json    # Permessi desktop
    mobile.json     # Permessi Android

client/src/
  tauri-api.js      # Bridge JS — wrapper dei comandi Tauri invoke()
```

## Relazione con LexFlow

Questa repo contiene **esclusivamente** il backend Rust e il bridge JavaScript.  
Il frontend React/Tailwind è nella repo principale [LexFlow](https://github.com/PieProton/LexFlow).
