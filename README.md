import { Card, CardContent } from "@/components/ui/card";
import { Button } from "@/components/ui/button";
import { Input } from "@/components/ui/input";
import { motion } from "framer-motion";
import { Sparkles, Ghost, Flame, ShoppingCart } from "lucide-react";
import Image from "next/image";

export default function VibeSecretaHomePage() {
  return (
    <div className="min-h-screen bg-gradient-to-b from-purple-950 via-purple-800 to-fuchsia-900 p-4 md:p-10 text-white">
      <header className="flex flex-col md:flex-row justify-between items-center mb-10">
        <h1 className="text-4xl font-extrabold text-fuchsia-300">Vibe Secreta</h1>
        <nav className="mt-4 md:mt-0 flex gap-4">
          <Button variant="ghost" className="text-white hover:text-fuchsia-400">Produtos</Button>
          <Button variant="ghost" className="text-white hover:text-fuchsia-400">Sobre</Button>
          <Button variant="ghost" className="text-white hover:text-fuchsia-400">Contato</Button>
          <Button variant="ghost" className="text-white hover:text-fuchsia-400 flex items-center gap-1">
            <ShoppingCart size={18} /> Carrinho
          </Button>
        </nav>
      </header>

      <section className="text-center mb-12">
        <motion.h2
          initial={{ opacity: 0, y: -20 }}
          animate={{ opacity: 1, y: 0 }}
          transition={{ duration: 0.8 }}
          className="text-3xl md:text-5xl font-bold text-fuchsia-200 mb-4"
        >
          Explore seu prazer com mistério e estilo.
        </motion.h2>
        <p className="text-lg text-fuchsia-100 max-w-xl mx-auto">
          Desperte sua vibe mais secreta com brinquedos, acessórios e sensações únicas.
        </p>
        <div className="mt-6">
          <Input placeholder="Receba segredos e descontos por e-mail ✨" className="max-w-md mx-auto mb-2 bg-white/10 border-white/20 placeholder-white" />
          <Button className="bg-fuchsia-600 hover:bg-fuchsia-700 text-white">Quero receber</Button>
        </div>
      </section>

      <section className="grid grid-cols-1 md:grid-cols-3 gap-6 mb-16">
        <Card className="bg-white/10 backdrop-blur-sm border border-white/10">
          <CardContent className="p-6">
            <div className="flex items-center gap-3 mb-4 text-fuchsia-200">
              <Flame /> <h3 className="text-xl font-semibold">Brinquedos</h3>
            </div>
            <p>Para explorar, sentir e se reinventar.</p>
          </CardContent>
        </Card>

        <Card className="bg-white/10 backdrop-blur-sm border border-white/10">
          <CardContent className="p-6">
            <div className="flex items-center gap-3 mb-4 text-fuchsia-200">
              <Ghost /> <h3 className="text-xl font-semibold">Discrição</h3>
            </div>
            <p>Entrega sigilosa, experiência inesquecível.</p>
          </CardContent>
        </Card>

        <Card className="bg-white/10 backdrop-blur-sm border border-white/10">
          <CardContent className="p-6">
            <div className="flex items-center gap-3 mb-4 text-fuchsia-200">
              <Sparkles /> <h3 className="text-xl font-semibold">Estilo</h3>
            </div>
            <p>Design moderno e sensações com identidade.</p>
          </CardContent>
        </Card>
      </section>

      <section>
        <h2 className="text-2xl font-bold text-center mb-6 text-fuchsia-200">Produtos em Destaque</h2>
        <div className="grid grid-cols-1 md:grid-cols-3 gap-6">
          <Card className="bg-white/10 backdrop-blur-sm border border-white/10">
            <CardContent className="p-6">
              <Image src="/images/bullet-vibe.jpg" alt="Vibrador Bullet" width={500} height={300} className="rounded-xl mb-4" />
              <h3 className="text-xl font-semibold text-fuchsia-100 mb-2">Vibrador Bullet Recarregável</h3>
              <p className="text-fuchsia-100 text-sm mb-2">Pequeno no tamanho, gigante no prazer. 10 modos de vibração, design discreto e potente para estimular onde quiser.</p>
              <p className="text-fuchsia-300 font-bold mb-4">R$ 130,00</p>
              <Button className="bg-fuchsia-700 hover:bg-fuchsia-800 text-white w-full">Adicionar ao Carrinho</Button>
            </CardContent>
          </Card>

          <Card className="bg-white/10 backdrop-blur-sm border border-white/10">
            <CardContent className="p-6">
              <
