# Descrição do Sistema

## Nome do Sistema
ADOP - Aplicativo de Organização Pessoal

## Visão Geral
O ADOP é uma plataforma que visa auxiliar a organização de tarefas diárias por meio de elementos de gamificação, direcionada ao público em geral. Desenvolvida com base em ferramentas que auxiliam indivíduos com Transtorno do Déficit de Atenção com Hiperatividade (TDAH) no desenvolvimento da habilidade de foco, a plataforma proporciona uma experiência interativa e gamificada. Dessa forma, busca-se promover um melhor desempenho pessoal e profissional, contribuindo para o crescimento e a autoestima do usuário.

## Funcionalidades Principais

- **Pontuação**: Motivação para o usuário manter sua consistência e disciplina na conclusão de tarefas.
- **Toque personalizado**: Por meio dos mesmos, ocorre o lembrete alertando que possui atividades a serem concluídas.
- **Relatórios**: Apresentam uma relação das conclusões de atividades e suas pontuações em um determinado período de tempo.
- **Tecnica de Pomodoro**: Gestão do tempo através da divisão de tarefas em intervalos de tempos fixos.

## Público-Alvo
O sistema é destinado ao público em geral, a partir dos 12 anos de idade, com atenção especial às necessidades de pessoas com Transtorno de Déficit de Atenção e Hiperatividade (TDAH).

## Tecnologias Utilizadas
- **Frontend**: React Native e Expo
- **Backend**: Firebase
- **Banco de Dados**: Firebase

## Arquitetura do Sistema
A arquitetura do sistema é baseada em uma abordagem serverless utilizando Backend como Serviço (BaaS), com o uso do Firebase como infraestrutura principal. Toda a lógica de backend, autenticação, banco de dados e notificações é gerenciada pelo Firebase, enquanto o aplicativo móvel é desenvolvido com React Native e Expo.

O sistema é escalável e modular, permitindo que os serviços da aplicação sejam utilizados sob demanda, sem a necessidade de gerenciar servidores. Isso facilita a escalabilidade automática conforme o número de usuários aumenta, reduz a complexidade de manutenção, já que grande parte da infraestrutura é gerenciada pela própria plataforma, e contribui para a segurança, aproveitando os recursos nativos do Firebase, como autenticação segura e regras de acesso ao banco de dados..

---