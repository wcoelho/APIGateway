# APIGateway
Gateway API para o aplicativo Music Experience. 
  
O API gateway foi feito em NodeJS, utilizando ExpressJS.  
A configuração (que pode ser vista no arquivo 'config/gateway.config.yml') foi feita para mapear todos os serviços referentes às APIs de usuários e avaliações e músicas (incluindo artistas, letras e playlists).  
Os serviços estão em servidores separados.  
- Usuários e Avaliações: http://localhost:5000 (https://github.com/wcoelho/UsersAndRatingsAPI). 
- Músicas: http://localhost:3001 (https://github.com/wcoelho/MusicsAPI).   
O caminho do gateway é: http://localhost:6001/api/v1/<servico>, expondo os seguintes serviços:  
- usuarios: operações relativas ao usuário.  
- avaliacoes: operacoes relativas à avaliação pelo usuário de músicas ou artistas.  
- musicas: busca músicas (integração com Spotify)  
- playlists: busca playlists do usuário (integração com Spotify)  
- letras: busca letras de músicas (integração com musixmatch)  
- artistas: operações relativas aos artistas.  
