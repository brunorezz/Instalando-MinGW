# 🧰 Guia Simplificado: Instalação e Uso do MinGW no VS Code

## 📦 1. Baixar e Instalar o MinGW
1. Acesse o site oficial: [https://osdn.net/projects/mingw/releases/](https://osdn.net/projects/mingw/releases/)
2. Baixe o instalador **mingw-get-setup.exe** e execute-o.
3. Na tela de componentes, marque:
   ```bash
   mingw32-gcc-g++
   ```
   (para compilar C e C++)
4. Vá em **Installation → Apply Changes** e aguarde o download e instalação.

---

## ⚙️ 2. Configurar a Variável de Ambiente (PATH)
1. Após instalar, vá até a pasta de instalação (geralmente `C:\MinGW\bin`).
2. Copie esse caminho.
3. No Windows, pesquise por **Editar variáveis de ambiente do sistema**.
4. Em “Variáveis do sistema”, selecione **Path → Editar → Novo** e cole o caminho.
5. Clique em **OK** para salvar.

---

## 🧪 3. Testar a Instalação
Abra o **Prompt de Comando** e digite:
```bash
gcc --version
```
Se aparecer a versão do GCC, o MinGW está instalado corretamente ✅.

---

## 💻 4. Configurar o VS Code
1. Instale a extensão **C/C++** (Microsoft).
2. Abra o terminal do VS Code com **Ctrl + `**.
3. Crie e salve um arquivo:
   - `main.c` → para C  
   - `main.cpp` → para C++
4. Compile o arquivo:
   ```bash
   gcc main.c -o main      # Para C
   g++ main.cpp -o main    # Para C++
   ```
5. Execute o programa:
   ```bash
   ./main
   ```

---

## 💡 Dica Extra
Você pode criar uma **tarefa automatizada** para compilar com um atalho:
- Vá em **Terminal → Configure Tasks → Create tasks.json**.
- Configure o comando de compilação para o seu projeto.

---

### 🧠 Observação
Este guia cobre apenas o uso básico do **MinGW** no VS Code.  
Perfeito para quem quer compilar e rodar programas em C/C++ de forma simples.
