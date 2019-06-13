# APIGateway
Gateway API para o aplicativo Music Experience. 
  
O API gateway foi feito em NodeJS, utilizando ExpressJS.  
A configuração foi feita para mapear todos os serviços referentes às APIs de usuários e avaliações e músicas (incluindo artistas e letras).  
Os serviços estão em servidores separados.  
- Usuários e Avaliações: http://localhost:5000. 
- Músicas: https://localhost:3001.   
O caminho do gateway é: http://localhost:6001/api/v1/<servico>, expondo os seguintes serviços:  
- usuarios: operações relativas ao usuário.  
- avaliacoes: operacoes relativas à avaliação pelo usuário de músicas ou artistas.  
- musicas: busca músicas (integração com Spotify)  
- playlists: busca playlists do usuário (integração com Spotify)  
- letras: busca letras de músicas (integração com musixmatch)  
- artistas: operações relativas aos artistas.  


