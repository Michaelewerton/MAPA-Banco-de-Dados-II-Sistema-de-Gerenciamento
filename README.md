
MAPA – Banco de Dados II: Sistema de Gerenciamento de Hospedagens Hoteleiras

Michael Ewerton Oliveira Disciplina: Banco de Dados II Instituição: UniCesumar

Descrição Geral do Projeto
Nesta atividade, foi desenvolvido um sistema completo de gerenciamento de hospedagens hoteleiras utilizando comandos SQL aplicados ao MySQL, com foco em estrutura de dados, manipulação de registros, procedimentos armazenados, funções personalizadas e triggers. A proposta simulou operações reais de reservas, check-ins, pagamentos e controle de quartos em dois hotéis fictícios.

Componentes Criados
Esquema e Tabelas
Criação do banco hospedar_db com tabelas:

Hotel: classificação, cidade, nome

Quarto: tipo, preço, vínculo com hotel

Cliente: CPF, e-mail, telefone

Hospedagem: datas, status, valor e vínculo com quarto e cliente

🏷Dados Inseridos
2 hotéis com 5 quartos cada

3 clientes simulados

20 hospedagens (5 para cada status: reserva, hospedado, finalizada, cancelada)

Consultas SQL Implementadas
Listagem geral de hotéis e seus respectivos quartos

Clientes com hospedagens finalizadas

Histórico cronológico de hospedagens por cliente

Cliente com maior número de hospedagens

Clientes com hospedagens canceladas

Receita total por hotel, ordenada decrescentemente

Clientes com reservas em hotel específico

Valor total gasto por cada cliente

Quartos sem hóspedes

Média de preços das diárias por tipo de quarto

Comandos de Alteração
Criação da coluna checkin_realizado (boolean) na tabela Hospedagem

Atualização com TRUE para hospedagens em andamento/finalizadas e FALSE para canceladas/reservas

Renomeação da coluna classificacao para ratting na tabela Hotel

Procedures Criadas
RegistrarCheckIn: altera status para “hospedado” e atualiza data

CalcularTotalHospedagem: calcula valor com base nas datas e preço da diária

RegistrarCheckout: atualiza data de saída e marca como “finalizada”

Funções Criadas
TotalHospedagensHotel(hotel_id) → retorna total de hospedagens por hotel

ValorMedioDiariasHotel(hotel_id) → retorna média das diárias do hotel

VerificarDisponibilidadeQuarto(quarto_id, data) → retorna TRUE ou FALSE

Triggers Criadas
AntesDeInserirHospedagem: verifica disponibilidade do quarto e cancela inserção se ocupado

AposDeletarCliente: registra exclusão em tabela de log para auditoria

Resultado da Avaliação
Avaliação concluída com êxito. Nota máxima e reconhecimento pela entrega correta e completa de todos os itens propostos. “Você conseguiu realizar o que era esperado na atividade. Continue se dedicando aos estudos!”
