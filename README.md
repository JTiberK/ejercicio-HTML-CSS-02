Ejercicio Práctico: Galería de Imágenes Responsiva

Vamos a crear una galería de imágenes que muestre 4 columnas en escritorio y 1 columna en móvil . Esto se logra
combinando CSS Grid con Media Queries.

Código Completo

/* Estilo base para la galería */

. galeria {
display: grid; /* Habilita el sistema de rejilla */

grid-template-columns: repeat(4, 1fr); /* 4 columnas iguales */

gap: 10px; /* Espacio entre las imágenes */

/* Media Query para móviles */

@media (max-width: 768px) {

.galeria {
grid-template-columns: 1fr; /* Cambia a 1 columna */
}


/* Estilo para las imágenes */

. galeria img {
max-width: 100%; /* Las imagenes se ajustan al contenedor */
height: auto;   /* Mantienen su proporcion */
