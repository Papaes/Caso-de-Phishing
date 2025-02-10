# 🛡️ Investigação de Caso de Phishing

📅 Data do Caso: 24/11/2024

🔍 Categoria: Análise Forense & Phishing Investigation

# 📌 Descrição do Caso
Um e-mail fraudulento foi enviado a um usuário, alegando uma multa pendente no valor de R$195 e solicitando pagamento via link suspeito. Após verificação no site oficial do DETRAN , não houve nenhuma multa registrada.

Para investigar o domínio fornecido no e-mail, foram utilizadas ferramentas como:

Nikto (para análise de vulnerabilidades no servidor)

cURL (para verificar o comportamento do site)

Whois (para obter informações sobre o registro do domínio)

# 🔎 Análises Realizadas

🖥️ 1. Resultados do Nikto

🔗 Domínio escaneado: @dominio.com

📍 Endereço IP: @dominio.com

# ✅ Problemas detectados:

❌ Ausência do título X-Frame-Options (vulnerável a ataques de clickjacking)

❌ Falta do cabeçalho Strict-Transport-Security (permite conexões inseguras)

❌ Content-Type ausente , aumentando o risco de ataques de MIME sniffing

❌ Redirecionamento suspeito para/avaliação fiscal/site1

# 📄 2. Resultados do Whois

🔍 Domínio: @dominio.com

👤 Proprietário: @Usuario.com

📧 E-mail registrado: email_oculto

🖥️ Provedor de DNS: todasolucao.com.br

📅 Criação do domínio: 30/11/2023

⏳ Expiração: 11/11/2025

⚠ Observação: O domínio não pertence a nenhuma entidade governamental e foi registrado recentemente, sendo comum de phishing.

🌐 3. Captura da Página Suspeita

📌 Título da página: "Aviso de Regularização Pendente"

💰 Valores apresentados:

Multa original: R$195,23

Com desconto: R$117,14

🔗 Botão malicioso: "Acessar Gov.br" (tentando simular um site oficial)

⚠️ O layout imita comunicações oficiais do Governo Brasileiro, mas o domínio não é legítimo.

# 📌 Conclusões

💡 Índices claros de Phishing:

✔️ Domínio fraudulento usado para golpes de engenharia social

✔️ Falta de cabeçalhos de segurança , tornando o site vulnerável

✔️ Domínio registrado por pessoa física , sem relação com órgãos governamentais

✔️ Técnicas de urgência no e-mail , instruídas o usuário a agir sem pensar

# 🛡️ Medidas Recomendadas

🔹 Nunca clique em links suspeitos antes de verificar a origem

🔹 Consulte o site oficial do órgão antes de tomar qualquer ação

🔹 Utilize ferramentas como Whoise Niktopara verificar as restrições de domínios

🔹 Mantenha uma mentalidade de "Think Before You Click"



📌 Autor: Mateus Costa Papaes


# ⚠️ Este estudo tem fins educacionais e não representa uma acusação contra qualquer pessoa ou entidade.
