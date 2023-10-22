# Transformando dados no Power BI

🔋 Etapas de Processamento:           
Foi criada uma instância na Azure para o MySQL; 

Criei o banco de dados com a base fornecida;

No momento de integração do Power BI com MySQL Azure, não consegui executar a etapa, tentei inúmeras vezes, instalei o conector, efetuei a regra no firewall, até tentei abrir o BD diretamente do navegador para o BI, mas sem sucesso. Nos arquivos constará print do BD feito na Azure, porém no BI não foi feita a conexão.

🗂️ Etapas de Transformação:  
Comecei transformando a variável "Salary" em Decimal, pois se referia ao salário;

Depois separei o endereço para que ele ficasse o mais atômico possível;

Logo após alterei o Super_Ssn de um funcionário que estava sem, considerei ele como gerente, visto que ele é o único presente no departamento 1;  

Na coluna "Hours" havia uma inconsistencia de dados 0 que mudei para um valor válido;

Após isso fiz as mesclas de departamento e localidade e nome dos funcionários;

Então mesclei as consultas a fim de ver os funcionários por departamento. Aqui utilizamos a mesclar colunas e não consultas pois os nossos dados estão numa mesma tabela, logo, não faria sentido e nem teria como efetuar essa operação;


Por fim, mesclei e agreguei para descobrir quantos funcionários possui cada gerente.
