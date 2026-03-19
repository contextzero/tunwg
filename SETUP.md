# Setup contextzero/tunwg

1. **Crear el repo en GitHub** (si no existe):
   ```bash
   gh repo create contextzero/tunwg --public --source=. --description "WireGuard in a tunnel"
   ```
   O crearlo en https://github.com/organizations/contextzero/repositories/new.

2. **Apuntar origin a contextzero y subir**:
   ```bash
   git remote set-url origin https://github.com/contextzero/tunwg.git
   git add -A && git commit -m "chore: contextzero fork, release workflow"
   git push -u origin main
   ```

3. **Primer release**: en GitHub → Actions → Release → Run workflow.  
   O crear un tag y hacer push: `git tag v1.0.0 && git push origin v1.0.0`.

Los binarios del release los usa nest (download-tunwg) desde `https://github.com/contextzero/tunwg/releases/latest/download/...`.
