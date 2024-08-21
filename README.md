# Exerc-cio-JOO
Nesse repositório esta lançado o desafio de criar um código em JAVA com as seguintes especificações encontradas no README
CRIAR UM CODIGO EM JAVA PARA REALIZAR O LOGIN E SENHA DE UM USUARIO DE UMA AGENCIA AEREA, APOS O LOGIN E SENHA O USUARIO DEVE INFORMAR, O CODIGO DEVE CONTER O NOME DO PASSAGEIRO, DOCUMENTO DE IDENTIFICACAO RG, CPF, NUMERO DO PASSAPORTE, TELEFONE DE CONTATO CONTENDO DDD MAIS O NUMERO, TELEFONE DE CONTATO DE EMERGENCIA NO MESMO FORMATO, DESTINO DEVE TER A OPCAO, EUA, PORTUGAL, AUSTRALIA, ITALIA, RUSSIA, CHINA, DATA DE IDA E VOLTA.

```java
import java.util.Scanner;

public class AgenciaAerea {

    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        // Realizar login
        System.out.println("Login da Agência Aérea");
        System.out.print("Usuário: ");
        String usuario = scanner.nextLine();
        System.out.print("Senha: ");
        String senha = scanner.nextLine();

        // Verificar login e senha
        if (autenticarUsuario(usuario, senha)) {
            System.out.println("Login bem-sucedido!");
```
continuem
coloque o trecho do código que vc fez e seu nome para identificar
------------- MArcus ------------------------

```java
public class Passageiro {
    private String nomePassageiro;
    private String rg;
    private String cpf;
    private String numeroPassaporte;
    private String telefoneContato;
    private String telefoneEmergencia;
    private String destino;
```


------------------------------- TIAGO ALVES ----------------
// COLETA DE DADOS DO PASSAGEIRO 
}
       Sytem.out.println ("Login bem-sucedido!")
       usuario passageiro = new Usuario(); 
       
       System.out.println("Digite o nome do do passageiro:");
       passageiro.setNome(scanner.nextLine());

       System.out.println("Digite RG do passageiro:);
       passageiro.setRg(scanner.nextLine());

       System.out.println("Digite o CPF do pasageiro:");
       passageiro.setCpf(scanner.nextLine());

       System.out.println("Digite o numero do passaporte do passageiro:");
       passageiro.setPassaporte(scanner.nextLine());

       System.out.println("Digite o telefone de contato (DDD + Numero):");
       passageiro.setTelefone(scanner.nextLine());

       System.out.println ("Digite o telefone de contato de emergencia (DDD + Numero):);
       passageiro.setTelefoneEmergencia(scanner.nextLine());

      Sytem.out.println("Escolha o destino (EUA, PORTUGAL, AUTRALIA, ITALIA, RUSSIA, CHINA):);
      passageiro.setDestino(scanner.nextLine());

      System.out.println("Digite a data de ida (formato AAAA-MM-DD):");
      passageiro.setDataIda(scanner.nextLine());

      System.out.println("Digite a data de volta (formato AAAA-MM-DD):");
      passageiro.setDataVolta(scanner.nextLine());
        
      // Mostrar dados coletados 
      System.out.println(" Dados do Passageiro: ");
      System.out.println(passageiro);
      }
------------------------------------------------------------------------------------
Continuem

$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$
Atividade colaborativa cada um deve comentar pelo menos 2 (duas) linhas do código
```java
import java.util.Scanner;

public class AgenciaAerea {

    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        // Realizar login
        System.out.println("Login da Agência Aérea");
        System.out.print("Usuário: ");
        String usuario = scanner.nextLine();
        System.out.print("Senha: ");
        String senha = scanner.nextLine();

        // Verificar login e senha
        if (autenticarUsuario(usuario, senha)) {
            System.out.println("Login bem-sucedido!");

            // Solicitar informações do passageiro
            System.out.print("Nome do passageiro: ");
            String nome = scanner.nextLine();

            System.out.print("Documento de Identificação (RG): ");
            String rg = scanner.nextLine();

            System.out.print("CPF: ");
            String cpf = scanner.nextLine();

            System.out.print("Número do Passaporte: ");
            String passaporte = scanner.nextLine();

            System.out.print("Telefone de Contato (com DDD): ");
            String telefoneContato = scanner.nextLine();

            System.out.print("Telefone de Emergência (com DDD): ");
            String telefoneEmergencia = scanner.nextLine();

            // Escolha do destino
            String[] destinos = {"EUA", "Portugal", "Austrália", "Itália", "Rússia", "China"};
            System.out.println("Destinos disponíveis:");
            for (int i = 0; i < destinos.length; i++) {
                System.out.println((i + 1) + ". " + destinos[i]);
            }
            System.out.print("Escolha o destino (número): ");
            int escolhaDestino = scanner.nextInt();
            scanner.nextLine(); 
            String destinoEscolhido = destinos[escolhaDestino - 1];

            // Datas de ida e volta
            System.out.print("Data de Ida (dd/mm/yyyy): ");
            String dataIda = scanner.nextLine();

            System.out.print("Data de Volta (dd/mm/yyyy): ");
            String dataVolta = scanner.nextLine();

            // Exibir informações
            System.out.println("\nInformações do Passageiro:");
            System.out.println("Nome: " + nome);
            System.out.println("RG: " + rg);
            System.out.println("CPF: " + cpf);
            System.out.println("Passaporte: " + passaporte);
            System.out.println("Telefone de Contato: " + telefoneContato);
            System.out.println("Telefone de Emergência: " + telefoneEmergencia);
            System.out.println("Destino: " + destinoEscolhido);
            System.out.println("Data de Ida: " + dataIda);
            System.out.println("Data de Volta: " + dataVolta);
        } else {
            System.out.println("Login ou senha incorretos. Acesso negado. Tente novamente!");
        }

        scanner.close();
    }

    // Método de autenticação simples
    private static boolean autenticarUsuario(String usuario, String senha) {
        // Aqui, podemos colocar uma validação simples
        return usuario.equals("passanger9") && senha.equals("pass9");
    }
}
```


