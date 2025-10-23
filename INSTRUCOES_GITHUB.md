# Como Publicar o Jogo no GitHub (Para Arquivos Grandes)

## ❗ Problema: Arquivos Maiores que 100MB

O GitHub **não aceita** arquivos individuais maiores que 100MB através do Git normal. O arquivo `jogo_blender.blend.exe` tem ~117MB.

## ✅ Soluções Disponíveis

### **Opção 1: GitHub Releases (RECOMENDADO - Mais Simples)**

Esta é a melhor opção para distribuir executáveis:

1. **Crie o repositório no GitHub** (sem marcar "Initialize with README")
2. **Faça o push do código** (sem o .exe):
   ```bash
   git push -u origin main
   ```

3. **Crie uma Release**:
   - No GitHub, vá em "Releases" → "Create a new release"
   - Escolha uma tag (ex: `v1.0`)
   - Título: "Jogo Blender v1.0"
   - Descrição: Descrição do jogo
   - **Arraste o arquivo `jogo_blender.blend.exe`** na seção "Attach binaries"
   - Clique em "Publish release"

4. Pronto! O executável estará disponível para download na página de Releases.

### **Opção 2: Git LFS (Large File Storage)**

Para manter o arquivo no repositório Git:

1. **Instale o Git LFS**:
   ```bash
   git lfs install
   ```

2. **Configure o Git LFS para arquivos .exe**:
   ```bash
   git lfs track "*.exe"
   ```

3. **Adicione o arquivo**:
   ```bash
   git add .gitattributes
   git add jogo_blender.blend.exe
   git commit -m "Adicionar executável com Git LFS"
   ```

4. **Faça o push**:
   ```bash
   git push -u origin main
   ```

⚠️ **Nota**: Git LFS tem limitações na conta gratuita do GitHub (1GB de armazenamento e 1GB de transferência por mês).

### **Opção 3: Upload Manual pelo Site**

1. Crie o repositório no GitHub
2. Faça upload apenas do código (sem arquivos grandes)
3. Para o executável, use Releases ou outro serviço de hospedagem (Drive, Dropbox, etc.)

## 📋 Comandos Rápidos

### Setup Inicial (Primeira vez)
```bash
git init
git add .
git commit -m "Primeira versão do jogo Blender"
```

### Conectar ao GitHub
```bash
git remote add origin https://github.com/SEU_USUARIO/NOME_DO_REPOSITORIO.git
git branch -M main
git push -u origin main
```

### Com Git LFS
```bash
git lfs install
git lfs track "*.exe"
git add .gitattributes jogo_blender.blend.exe
git commit -m "Adicionar executável"
git push
```

## 🎯 Recomendação Final

Use **GitHub Releases** para o executável. É mais simples e não tem limitações de tamanho para arquivos individuais.
