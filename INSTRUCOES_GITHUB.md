# Instruções para Postar no GitHub

## Opção 1: Usando GitHub Desktop (Mais Fácil)

1. Baixe o GitHub Desktop: https://desktop.github.com/
2. Faça login na sua conta GitHub
3. Clique em "File" > "Add Local Repository"
4. Escolha a pasta `jogo_blender`
5. Clique em "Publish repository"
6. Escolha o nome do repositório
7. Marque "Keep this code private" se quiser manter privado
8. Clique em "Publish repository"

## Opção 2: Usando Git pelo Terminal

1. Abra o PowerShell na pasta do projeto
2. Execute os seguintes comandos:

```bash
# Inicializar o repositório Git
git init

# Adicionar todos os arquivos
git add .

# Fazer o commit inicial
git commit -m "Primeira versão do jogo Blender"

# Criar repositório no GitHub (acesse github.com e crie um novo repositório)
# Depois execute:
git remote add origin https://github.com/SEU_USUARIO/NOME_DO_REPOSITORIO.git
git branch -M main
git push -u origin main
```

## Opção 3: Upload Manual pelo Site

1. Acesse https://github.com/new
2. Crie um novo repositório
3. Clique em "uploading an existing file"
4. Arraste a pasta do projeto inteira
5. Clique em "Commit changes"

## ⚠️ Observação Importante

O arquivo `.gitignore` foi criado para evitar upload de arquivos desnecessários. 
Se o repositório ficar muito grande, você pode considerar:

- Fazer upload apenas do executável (`jogo_blender.blend.exe`)
- Criar releases com downloads do jogo
- Usar Git LFS para arquivos grandes

