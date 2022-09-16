```c#

void Start()
   {
       this.arvoreHabilidades = new SkillTree(false, "Nome");    

       Skill hab_ini_1 = new Skill(1, "A");
       Skill hab_1_1 = new Skill(2, "AA");
       Skill hab_1_2 = new Skill(3, "AAA");
       Skill hab_1_3 = new Skill(4, "AAAA");
       Skill hab_1_4 = new Skill(4, "AAAB");

       hab_ini_1.InserirPosteior(hab_1_1);
       hab_ini_1.InserirPosteior(hab_1_2);
       hab_ini_1.InserirPosteior(hab_1_3);
       hab_1_2.InserirPosteior(hab_1_4);

       this.arvoreHabilidades.AdicionarHabilidadeInicial(hab_ini_1);

       //void AjustarConsumoArvore()
       //Ajusta as Skill para o tipo de consumo definido para a arvore
       this.arvoreHabilidades.AjustarConsumoArvore();


```
      ![1](https://user-images.githubusercontent.com/92062346/190831261-9a046352-ec57-4c14-b0ef-bbc46f04681d.png)

```c#









       this.arvoreHabilidades = new SkillTree();

       List<string> habilidades = new List<string>();
       habilidades.Add("A");
       habilidades.Add("B");
       habilidades.Add("C");
       this.arvoreHabilidades.CriarRamo(habilidades, false, multiplicadorPontuacao: 2);

       List<string> habilidades2 = new List<string>();
       habilidades2.Add("B");
       habilidades2.Add("B1");
       habilidades2.Add("B2");
       this.arvoreHabilidades.CriarRamo(habilidades2, false, pontuacaoInicial: 1);














       this.arvoreHabilidades = new SkillTree();

       List<string> habilidades = new List<string>();
       habilidades.Add("A");
       habilidades.Add("B");
       habilidades.Add("C");
       this.arvoreHabilidades.CriarRamo(habilidades, false, multiplicadorPontuacao: 2);


       List<string> habilidades2 = new List<string>();
       habilidades2.Add("B");
       habilidades2.Add("B1");
       habilidades2.Add("B2");

       this.arvoreHabilidades.CriarRamo(habilidades2, false, pontuacaoInicial: 1);

       Skill hablidadeJaCriada = this.arvoreHabilidades.ObterHabilidadeNome("B3");
       Skill habNova = new Skill(5, "B1");
       hablidadeJaCriada.InserirPosteior(habNova);









       //public Skill(int pontuacaoNecessaria, string nomeHabilidade, bool precisaTodosAntecessores = false)
       //public int Ativar(int pontuacaoPlayer)
       //public bool Ativa()
       //public bool PodeAtivar(int pontuacaoPlayer)
       //public List<Skill> AntecessoresAtivos()
       //public bool InserirAntecessor(Skill habilidade)
       //public bool InserirPosteior(Skill habilidade)
       //public bool PrecisaTodosAntecessores(bool precisaTodosAntecessores)
       //public bool DefinePrecisaTodosAntecessores(bool precisaTodosAntecessores)
       //public RetornoNecessidadesHabilidade NecessidadesHabilidade()
       //    public class RetornoNecessidadesHabilidade
       //    {
       //        public List<Skill> necessarios = new List<Skill>();
       //        public int pontuacaoNecessaria = 0;
       //        public bool precisaTodosAntecessores = false;

       //        public RetornoNecessidadesHabilidade(List<Skill> necessarios, int pontuacaoNecessaria, bool precisaTodosAntecessores)
       //        

       //    }
       //public void DefinirAntecessores(List<Skill> antecessores)
       //public void RemoverAntecessor(Skill antecessor)
       //public void RemoverPosterior(Skill posterior)
       //public void RemoverHabilidade(Skill habilidade)
       //public List<Skill> Antecessores()
       //public List<Skill> Posteriores()
       //public string Nome()
       //public void DefinirNome(string nomeHabilidade)
       //public void DefinirConsumo(bool custoConsumo)
       //public void DefinirPontuacaoNecessariao(int pontuacaoNecessaria)
       //public int QuantosPontosFaltam(int pontuacaoPlayer)
       //public int QuantasHabilidadesFaltam(int pontuacaoPlayer)
       //public bool PossuiAtributo(string nome, object atributo)
       //public void AddAtributo(string nome, object atributo)
       //public void AddAtributos(string nome, List<object> atributos)
       //public void DefinirAtributos(string nome, List<object> atributos)
       //public Dictionary<string, List<object>> Atributos()

       //--------------------------------
       //public SkillTree(bool custoConsumo = false, string nomeArvore = "")
       //public bool AdicionarHabilidadeInicial(Skill habilidade)
       //public bool AdicionarHabilidadeFinal(Skill habilidade)
       //public void ListarHabilidadesAtivas()
       //public List<Skill> HabilidadesIniciais()
       //public List<Skill> HabilidadesFinais()
       //public List<Skill> Habilidades()
       //public List<Skill> HabilidadesAtivas()
       //public List<Skill> HabilidadesInativas()
       //public bool TemHabilidade(Skill habilidade)
       //public bool HabilidadeAtiva(Skill habilidade)
       //public void DefinirConsumo(bool custoConsumo)
       //public void AjustarConsumoArvore()
       //public Skill ObterHabilidadeNome(string nome)
       //public bool CriarRamo(List<string> habilidades, bool custoConsumo = false, int pontuacaoInicial = 1, int somadorPontuacao = 1, int multiplicadorPontuacao = 0)
       //public void DeletarHabilidadeNome(string nomeHabilidade)
       //public bool PossuiAtributo(string nome, object atributo)
       //public bool PossuiAtributoAtivo(string nome, object atributo)

   }



```
