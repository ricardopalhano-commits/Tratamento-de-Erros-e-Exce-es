function dividir(a: number, b: number): number {
  if (b === 0) {
    throw new Error("Não é possível dividir por zero.");
  }

  return a / b;
}

const entrada = require("fs").readFileSync(0, "utf8").trim();
const divisor = Number(entrada);

try {
  if (entrada === "" || !Number.isFinite(divisor)) {
    throw new Error("Informe um número válido.");
  }

  const resultado = dividir(10, divisor);
  console.log(`Resultado: ${resultado}`);
} catch (erro: unknown) {
  if (erro instanceof Error) {
    console.error(`Ocorreu um erro: ${erro.message}`);
  } else {
    console.error("Ocorreu um erro desconhecido.");
  }
} finally {
  console.log("Operação finalizada.");
}
