# Kapitalo — copie de secours du modèle de Kapi IA

Ce dépôt garde une copie **à l'identique** du modèle qu'utilise Kapi IA,
le conseiller de l'application Kapitalo. L'application télécharge d'abord
le modèle depuis sa source officielle ; elle ne vient ici que si cette
source ne répond pas.

## Le modèle

- **Gemma 4 E2B** (Google), format LiteRT-LM : `gemma-4-E2B-it.litertlm`
- Source officielle : [litert-community/gemma-4-E2B-it-litert-lm](https://huggingface.co/litert-community/gemma-4-E2B-it-litert-lm),
  révision `3d48132a00cf76de57d926de30f5c5c5ed9b8c0d`
- Licence : **Apache 2.0** (texte joint : `LICENSE-Apache-2.0.txt`).
  Le fichier n'est pas modifié.

## Les fichiers

GitHub limite chaque fichier à 2 Go : le modèle (2 588 147 712 octets) est
coupé en deux moitiés, à recoller dans l'ordre.

| Fichier | Octets | SHA-256 |
|---|---|---|
| `gemma-4-E2B-it.litertlm.partie1` | 1 294 073 856 | `99bef3d84fdddc99169ec12d7d4926e3fb3ff2153f70818364f979b86ad48035` |
| `gemma-4-E2B-it.litertlm.partie2` | 1 294 073 856 | `a9a4f91ab2e0192f9f5c163f31cedf37be3f3521e67f429f9706a7b6117e246f` |
| **Modèle recollé** | 2 588 147 712 | `181938105e0eefd105961417e8da75903eacda102c4fce9ce90f50b97139a63c` |

Recoller (Linux / macOS) : `cat gemma-4-E2B-it.litertlm.partie1 gemma-4-E2B-it.litertlm.partie2 > gemma-4-E2B-it.litertlm`

L'application vérifie l'empreinte du modèle recollé avant de l'utiliser :
un fichier différent ne s'installe jamais.

---

# Kapitalo — backup copy of the Kapi AI model

An **unmodified** copy of the Gemma 4 E2B model (Google, Apache 2.0
license) used by Kapi AI in the Kapitalo app, split in two halves (GitHub's
2 GB file limit). The app only uses it when the official source does not
respond, and checks the SHA-256 of the rebuilt file before using it.
