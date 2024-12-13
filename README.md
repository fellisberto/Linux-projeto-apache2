# Linux-projeto-apache2
Projeto DIO

Atualização do servidor:

O script inicia atualizando a lista de pacotes disponíveis no servidor com o comando apt-get update. Em seguida, ele atualiza todos os pacotes instalados no sistema para a última versão disponível usando apt-get upgrade -y. O parâmetro -y garante que o script responda automaticamente "sim" a qualquer pergunta durante o processo de atualização.

Instalação de pacotes:

O script instala dois pacotes essenciais:

Apache2: Um servidor web que permite que o site seja acessado pela internet.

Unzip: Uma ferramenta para descompactar arquivos no formato ZIP.

Download e instalação da aplicação:

O script baixa o arquivo ZIP da aplicação no GitHub usando o comando wget, salvando-o no diretório /tmp. Em seguida, descompacta o arquivo com unzip e copia os arquivos para o diretório /var/www/html, onde o Apache2 hospeda arquivos web.

Resumo das ações:

O script exibe duas mensagens informativas:

"Atualizando o servidor...": Indica que os pacotes do sistema estão sendo atualizados.

"Baixando e copiando os arquivos da aplicação": Informa que a aplicação está sendo baixada do GitHub e os arquivos estão sendo copiados para o diretório apropriado.

Observações:

O script pressupõe que o Git já está instalado no servidor.

Ele baixa a versão mais recente da aplicação do GitHub. Para instalar uma versão específica, é necessário editar o comando wget.

O script sobrescreve qualquer arquivo existente no diretório /var/www/html.

Conclusão:

O script automatiza a atualização do servidor e a instalação da aplicação, tornando o processo mais rápido e fácil, além de minimizar erros humanos.
