# Devops

Criar projeto
```
go mod init webserverfc
```

Testar a imagem criada
```
docker run --rm -p 8080:8080 lkosaka/gitopsfc:latest
```

Alterando tag com Kustomize
```
cd k8s
kustomize edit set image goserver=lkosaka/gitopsfc:novaTag
```