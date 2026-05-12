# Tienda de Perritos - Innovatech Chile

Este proyecto consiste en una aplicación de microservicios (Frontend, Backend y Base de Datos) desplegada de forma automatizada mediante CI/CD en AWS.

## Estructura del Proyecto
- **Frontend**: React/Node.js (Puerto 80)
- **Backend**: Node.js API (Puerto 3001)
- **Base de Datos**: MySQL 8.0 (Puerto 3306)

## Despliegue con Docker Compose
Para levantar el stack completo localmente o en la instancia EC2:
```bash
docker-compose up -d



### 3. El "Trigger" de la rama `deploy` (20%)
Recuerda lo que decía el PDF: el pipeline debe activarse al hacer push en la rama **`deploy`**.
* **Si ya lo hiciste en `main`**: No te preocupes tanto, pero si puedes, crea la rama `deploy` (`git checkout -b deploy`), cambia en tu archivo `.yml` la parte de `branches: [ "main" ]` por `branches: [ "deploy" ]` y haz el push. Así cumples el requisito al pie de la letra.

---

### ¿Cómo saber si ya terminaste? (Checklist Final)
Si puedes decir "SÍ" a todo esto, estás listo para el 7.0:
1. [ ] ¿Los 3 contenedores aparecen en `docker ps` en la EC2?
2. [ ] ¿El archivo `docker-compose.yml` tiene la sección `volumes:` al final?
3. [ ] ¿Tu Dockerfile del Backend tiene la línea `USER node`?
4. [ ] ¿Escribiste el `README.md`?
5. [ ] ¿Puedes entrar a la web desde tu navegador y ver que funciona?

**¿Hay algo de este checklist que todavía te genere dudas?** Si no, ¡ya estás listo para triunfar en la entrega!