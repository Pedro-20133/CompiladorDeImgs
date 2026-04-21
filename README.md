# 🎨 Compilador de Imgs (Pixel Art Renderer)

O **Compilador de Imgs** é uma ferramenta desktop desenvolvida em **Go**, utilizando a biblioteca **Fyne**, concebida para interpretar e renderizar artes em pixels a partir de ficheiros de configuração JSON.

Este projeto permite converter definições estruturadas (cores, posição e transparência) numa representação visual imediata.

---

## 🚀 Funcionalidades
* **Renderização Dinâmica:** Converte ficheiros JSON contendo matrizes de pixels em elementos visuais (retângulos) no ecrã.
* **Validador de Projetos:** Verifica a integridade dos ficheiros JSON carregados (valida nome, data e presença de dados de pixel).
* **Interface Gráfica Intuitiva:** Desenvolvido com **Fyne**, oferecendo uma experiência de utilizador limpa e funcional.
* **Controlo de Opacidade:** Suporte nativo para aplicar canais de transparência (alfa) às cores definidas no JSON.

---

## 📋 Estrutura do Ficheiro JSON
O programa espera um ficheiro JSON com a seguinte estrutura:

```json
{
  "name": "Configuração de Iluminação",
  "description": "Exemplo de mapeamento de pixels LED",
  "date": "2026-04-20",
  "pixels": [
    {
      "pos": 1,
      "transparence": 0.5,
      "color": "255, 0, 0"
    },
    {
      "pos": 2,
      "transparence": 0.8,
      "color": "0, 255, 0"
    },
    {
      "pos": 3,
      "transparence": 1.0,
      "color": "0, 0, 255"
    }
  ]
}
