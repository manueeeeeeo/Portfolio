<template>
    <section id="contact" class="my-12 animate-fade-in">
      <h2 class="text-3xl font-semibold mb-4">Contacto</h2>
      <form
        action="https://formsubmit.co/tuemail@ejemplo.com"
        method="POST"
        class="grid gap-4 max-w-md"
      >
        <input type="text" name="name" placeholder="Nombre" required class="p-2 border rounded" />
        <input type="email" name="email" placeholder="Email" required class="p-2 border rounded" />
        <textarea name="message" placeholder="Mensaje" required class="p-2 border rounded"></textarea>
        <button type="submit" class="bg-blue-600 text-white px-4 py-2 rounded hover:bg-blue-700">Enviar</button>
      </form>
    </section>
  </template>
  