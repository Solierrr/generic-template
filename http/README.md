# Coleção Bruno: generic-template

Abra a pasta `http/` como uma coleção Bruno e selecione o ambiente `local`. Ajuste a URL base em `environments/local.bru` para a porta usada pelo serviço.

Organize as requisições em subpastas por domínio ou recurso e use nomes numerados no formato `NNN-verbo-rota.bru`, como nos serviços Solaria. Marque no nome com `[mutates]` as operações que criam, atualizam, removem dados, iniciam fluxos ou chamam rotas internas. Inclua em `docs {}` o efeito relevante da operação para que quem for executá-la possa revisar antes.

Credenciais, tokens e chaves de API devem ficar vazios no ambiente versionado. Preencha-os localmente no Bruno e não faça commit desses valores. Use IDs de exemplo sintaticamente válidos e substitua-os por IDs existentes no banco local quando necessário.

A coleção não executa requisições automaticamente. Confira o efeito de cada chamada antes de enviá-la e mantenha os exemplos alinhados ao contrato real da API. Consulte o template canônico em [`docs-warehouse/templates/http/`](https://github.com/Solierrr/docs-warehouse/tree/main/templates/http).
