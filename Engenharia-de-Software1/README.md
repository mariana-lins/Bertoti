# ATIVIDADE 1
Texto 1

We see three critical differences between programming and software engineering: time, scale, and the trade-offs at play. On a software engineering project, engineers need to be more concerned with the passage of time and the eventual need for change. In a software engineering organization, we need to be more concerned about scale and efficiency, both for the software we produce as well as for the organization that is producing it. Finally, as software engineers, we are asked to make more complex decisions with higher-stakes outcomes, often based on imprecise estimates of time and growth.

Programação e engenharia de software são diferentes, a engenharia foca em tempo, escalabilidade e eficiência, exigindo decisões complexas e planejamento para mudanças futuras, enquanto a programação é mais voltada para a criação de código em si.

Texto 2 

Within Google, we sometimes say, “Software engineering is programming integrated over time.” Programming is certainly a significant part of software engineering: after all, programming is how you generate new software in the first place. If you accept this distinction, it also becomes clear that we might need to delineate between programming tasks (development) and software engineering tasks (development, modification, maintenance). The addition of time adds an important new dimension to programming. Cubes aren’t squares, distance isn’t velocity. Software engineering isn’t programming.

A engenharia de software vai além da simples criação de um software; envolve também seu desenvolvimento, modificação e manutenção. Trata-se de um campo que abrange muito mais do que apenas programação, focando na busca constante por inovações tecnológicas e na adaptação a novas demandas, sempre priorizando a qualidade e a eficiência.

# ATIVIDADE 2 
Desempenho vs. Escalabilidade:
Desempenho: Focar em otimizar a velocidade e a eficiência do sistema para um número limitado de usuários.
Escalabilidade: Priorizar a capacidade do sistema de suportar um aumento significativo no número de usuários, o que pode comprometer o desempenho em situações de carga elevada.

Segurança vs. Usabilidade:
Segurança: Implementar medidas rigorosas de segurança, como autenticações complexas, que podem dificultar o acesso do usuário.
Usabilidade: Criar uma interface simples e intuitiva que facilite o uso, mas que pode expor o sistema a vulnerabilidades.

Manutenibilidade vs. Performance:
Manutenibilidade: Adotar práticas de codificação que favoreçam a facilidade de manutenção e atualização do software, o que pode resultar em uma performance inferior.
Performance: Optar por otimizações que melhoram o desempenho imediato do sistema, mas que tornam o código mais complexo e difícil de manter no longo prazo.

# ATIVIDADE 3
![image](https://github.com/user-attachments/assets/7eb13462-bb43-4b91-aff4-069ae2450637)

Desempenho vs Escalabilidade:
Vejo que eles têm componentes específicos, como o "Timeline Scorer" e o "Timeline Service", para lidar com o alto volume de conteúdo e usuários. Parece que estão buscando equilibrar o desempenho em momentos de pico com a capacidade de escalar o sistema.

Segurança vs Usabilidade:
Embora não haja detalhes sobre segurança, é provável que tenham que encontrar um balanço entre proteger o sistema e fornecer uma experiência de usuário fluida e acessível.

Modularidade vs Acoplamento:
A arquitetura parece ser bastante modular, com vários serviços interconectados. Isso deve trazer benefícios de flexibilidade, mas também pode gerar desafios de acoplamento entre os módulos.

# ATIVIDADE 4
![image](https://github.com/user-attachments/assets/48b31c20-e35e-4113-b33a-2a6771dd078c)

~~~java
class Conta {
    private int agencia;
    private int contaCorrente;
    private float saldo;

    public void depositar(float valor) {
        this.saldo += valor;
    }

    public void sacar(float valor) {
        this.saldo -= valor;
    }

    public float getSaldo() {
        return this.saldo;
    }
}

class ContaPoupanca extends Conta {
    private int diaDeposito;

    public void verificarVencimento(int diaAtual) {
        if (diaAtual != this.diaDeposito) {
        }
    }
}

class Cliente {
    private int cpf;
    private String nome;
    private String telefone;

    public void mostrarCPF() {
    }

    public void verificarSaldo(Conta conta) {
        System.out.println("Saldo da conta: " + conta.getSaldo());
    }
}

~~~

