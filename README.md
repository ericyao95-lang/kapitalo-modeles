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
coupé en 12 morceaux égaux, `.01` à `.12`, à recoller dans l'ordre (dans la
version [gemma-4-e2b-v1](https://github.com/ericyao95-lang/kapitalo-modeles/releases/tag/gemma-4-e2b-v1)).

| Fichier | Octets | SHA-256 |
|---|---|---|
| `gemma-4-E2B-it.litertlm.01` | 215 678 976 | `0cfaf5b257e5e5cfca54ad38da9f2e97799437ca9523bf3170632cbf944623fe` |
| `gemma-4-E2B-it.litertlm.02` | 215 678 976 | `45dbe672a3333a470b42973d80f5d33d1587d13dfa43c0214197a4bd934d1579` |
| `gemma-4-E2B-it.litertlm.03` | 215 678 976 | `1ea5ecc289a84a563dbc9e56095439c7a8ae9e8578a720c02576e999ffa83035` |
| `gemma-4-E2B-it.litertlm.04` | 215 678 976 | `3f756a9b377ab0896668c4fe81a6b561486d4699c40ca3c729d9b54b1a7ac4d1` |
| `gemma-4-E2B-it.litertlm.05` | 215 678 976 | `7bd44c9f4817b2f94522db133107c81c07df654b54ec05bf141ebc0407687c85` |
| `gemma-4-E2B-it.litertlm.06` | 215 678 976 | `549b50bf1cbcc2bcf46b213ed3c5e63c299afcdcb23eeb633d0203b8f278766e` |
| `gemma-4-E2B-it.litertlm.07` | 215 678 976 | `6748e3c11ade140ffcdef60aa2f8140242f1a47e5648eb525620eb6fa394a0c3` |
| `gemma-4-E2B-it.litertlm.08` | 215 678 976 | `6cb0054f05faed51bd85ae5b0146ab501919a1ee451244a6e7c6c1e91ebe7451` |
| `gemma-4-E2B-it.litertlm.09` | 215 678 976 | `ca4373111e0cc82c4f58ff4cc1c6ce7826defb62261c62d6cd06aefc4949a816` |
| `gemma-4-E2B-it.litertlm.10` | 215 678 976 | `04da2e2ec0fab537ff03af6311954abe69bfeb96a1cde2e71cb5d3471dec6d06` |
| `gemma-4-E2B-it.litertlm.11` | 215 678 976 | `5572f93e7b6436240ca20a8136642eb2b960f47a9c96fb69e026d0ab246a15ad` |
| `gemma-4-E2B-it.litertlm.12` | 215 678 976 | `d2624c97a74196c5c78f937a0398575b7687058954d226fdb270c32d828c5515` |
| **Modèle recollé** | 2 588 147 712 | `181938105e0eefd105961417e8da75903eacda102c4fce9ce90f50b97139a63c` |

Recoller (Linux / macOS) : `cat gemma-4-E2B-it.litertlm.?? > gemma-4-E2B-it.litertlm`

L'application vérifie l'empreinte du modèle recollé avant de l'utiliser :
un fichier différent ne s'installe jamais.

---

# Kapitalo — backup copy of the Kapi AI model

An **unmodified** copy of the Gemma 4 E2B model (Google, Apache 2.0
license) used by Kapi AI in the Kapitalo app, split in 12 equal pieces
(GitHub's 2 GB file limit). The app only uses it when the official source does not
respond, and checks the SHA-256 of the rebuilt file before using it.
