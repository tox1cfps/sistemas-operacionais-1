# EVOLUÇÃO E ESTRUTURA DOS SISTEMAS OPERACIONAIS


Relatório técnico apresentado à disciplina de Sistemas Operacionais, como requisito parcial para avaliação acadêmica.

São Paulo  
2026  

---

## 1 INTRODUÇÃO

O sistema operacional constitui o principal software de um sistema computacional, sendo responsável pela gerência direta dos recursos de hardware, tais como CPU, memória principal, dispositivos de armazenamento e interfaces de rede.

Sua estrutura é organizada em torno de um componente central denominado **núcleo (kernel)**, que executa funções críticas de controle e coordenação do sistema.

Para garantir estabilidade e segurança, o sistema operacional opera em dois níveis distintos de privilégio:

- **Modo Usuário:** aplicações com acesso restrito.
- **Modo Kernel:** acesso completo ao hardware.

A comunicação entre programas e o núcleo ocorre por meio de **chamadas de sistema (*system calls*)**.

---

## 2 DESENVOLVIMENTO

### 2.1 Estruturas e Arquiteturas de Sistemas Operacionais

- **Sistemas Monolíticos:** núcleo compilado em bloco único; alta eficiência, manutenção mais complexa.
- **Sistemas em Camadas:** organização hierárquica com modularidade.
- **Máquinas Virtuais:** execução simultânea de múltiplos SOs sobre o mesmo hardware.
- **Modelo Cliente-Servidor (Micronúcleo):** núcleo mínimo com serviços executados em modo usuário.

### 2.2 Classificação quanto ao Processamento

- **Monoprogramáveis (Monotarefa):** executam um programa por vez.
- **Multiprogramáveis (Multitarefa):** compartilham recursos entre múltiplos processos.

Podem ser:
- **Tempo Compartilhado:** uso de *time-slice*.
- **Tempo Real:** prazos rígidos de resposta e controle de prioridade.

### 2.3 Sistemas com Múltiplos Processadores

- **Fortemente Acoplados:** compartilham memória e um único SO.
  - **SMP (Simétricos):** mesmo nível de acesso.
  - **Assimétricos:** processador mestre coordena os demais.

- **Fracamente Acoplados:** cada nó possui memória e SO próprios, comunicando-se via rede.
  - Sistemas Operacionais de Rede
  - Sistemas Distribuídos

---

## 3 CONCLUSÃO

A evolução dos sistemas operacionais demonstra uma tendência à multiprogramação e ao uso eficiente de múltiplos processadores.

A escolha da arquitetura impacta diretamente manutenção, segurança e robustez do sistema.

---

## REFERÊNCIAS

BARBOSA, Cynthia da Silva. **Sistemas operacionais**. Londrina: Editora e Distribuidora Educacional S.A., 2018.