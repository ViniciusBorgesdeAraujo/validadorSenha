### **validadorSenha - Biblioteca Java para Validação de Senhas**  

Bem-vindo ao repositório da biblioteca **validadorSenha**! 🚀  
Esta biblioteca foi projetada para validar senhas de maneira simples e eficiente, garantindo a segurança ao verificar critérios como comprimento, letras maiúsculas/minúsculas, números e caracteres especiais.  

---

## **📜 Funcionalidades**
- Verifica se a senha atende os seguintes requisitos:  
  - Pelo menos 8 caracteres.  
  - Contém letras maiúsculas e minúsculas.  
  - Inclui pelo menos um número.  
  - Possui um caractere especial (ex: `@`, `#`, `$`).  
- Fornece mensagens detalhadas para senhas inválidas.  

---

## **📂 Estrutura do Projeto**
```plaintext
src
└── br
    └── com
        └── validador
            └── validadorSenha.java
```

---

## **🚀 Como Usar**
### 1. **Compilar o Código**
No terminal, execute:  
```bash
javac -encoding UTF-8 -d ./bin ./src/br/com/validador/validadorSenha.java
```  

### 2. **Gerar o Arquivo JAR**
Crie o pacote JAR:  
```bash
jar cf validadorSenha.jar -C ./bin .
```  

### 3. **Integrar no Projeto**
Adicione o arquivo `validadorSenha.jar` ao classpath do seu projeto.  

---

## **🛠️ Exemplo de Uso**
```java
import br.com.validador.validadorSenha;

public class TesteValidador {
    public static void main(String[] args) {
        String senha = "Senha@123";

        try {
            boolean senhaValida = validadorSenha.validarSenha(senha);
            if (senhaValida) {
                System.out.println("Senha válida!");
            }
        } catch (IllegalArgumentException e) {
            System.out.println("Erro: " + e.getMessage());
        }
    }
}
```

---

## **🧰 Tecnologias Utilizadas**
- **Java 11+**
- **Compilador:** `javac`
- **Empacotador:** `jar`  

---

## **📜 Licença**
Este projeto está licenciado sob a [MIT License](LICENSE).  

---
