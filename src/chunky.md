# Chunky

Chunky allows you to pregenerate the chunks of a world. On CPUs with very few
threads, this can massively increase performance as the server doesn't have to
generate new terrain.

If we do all the heavy computation in generating the chunks *before* players
join the server, they can explore the world with little delay in chunks being
loaded.

