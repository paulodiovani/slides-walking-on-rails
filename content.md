<!-- .slide: data-background="linear-gradient(rgba(0, 0, 0, 0.65), rgba(0, 0, 0, 0.65)), url(img/railway.jpg)" data-background-size="cover" -->

## Andando sobre trilhos

Uma apresentação sobre o _ecossistema_ de _**Ruby on Rails**_.

<small>Versão 0.1.0</small>

<small>por Paulo Diovani</small>

Note:
Image credits: lemerg.com

====

![avatar][avatar] <!-- .element: class="img-half-right" -->

### <i class="fa fa-user"></i> Paulo Diovani Gonçalves

Tecnólogo em Sistemas para Internet pela Universidade Feevale.
Desenvolvedor na Codeminer 42.
Usuário GNU/Linux

[blog.diovani.com][blog]

[slides.diovani.com][slides]

[![codeminer42][code-logo]][code-site] <!-- .element: class="no-border no-background" -->

[avatar]: img/avatar.jpg
[blog]: http://blog.diovani.com
[slides]: http://slides.diovani.com
[code-logo]: img/codeminer42.png
[code-site]: http://codeminer42.com/

----

![code-main-logo][code-main-logo] <!-- .element: class="no-border no-background" style="width:480px" -->

estamos contratando

[become@codeminer42.com][become]

[code-main-logo]: img/codeminer.svg
[become]: mailto:become@codeminer42.com

====

## <i class="br br-codeminer"></i> Codeminer 42

- Processo ágil
- Foco em qualidade
- Times auto gerenciados
- Consultoria + Desenvolvimento
- Comunicação direta com o cliente

====

## <i class="fa fa-apple"></i> <i class="fa fa-linux"></i> prepare
## <i class="br br-ruby"></i> <i class="br br-rails"></i> develop
## <i class="fa fa-github"></i> <i class="br br-travis-ci"></i> commit/test
## <i class="br br-heroku"></i> <i class="br br-postgresql"></i> deploy

----

# <i class="br br-ruby"></i> <i class="br br-rails"></i>

# Primeiras impressões

Note:
Vindo do PHP, Javascript, Java e C#...

====

## <i class="br br-ruby"></i> Código "limpo" e legível

```ruby
# Output "I love Ruby"
say = "I love Ruby"
puts say

# Output "I *LOVE* RUBY"
say['love'] = "*love*"
puts say.upcase

# Output "I *love* Ruby"
# five times
5.times { puts say }
```

Note:
A maiorias dos métodos e construção de ruby
se assemelha muito a linguagem natural

====

## <i class="br br-ruby"></i> RubyGems

http://rubygems.org

- Gerenciador de pacotes do Ruby
- Formato padrão para distribuir programas e bibliotecas Ruby

====

## <i class="br br-ruby"></i> Bundler

```bash
gem install bundler
vim Gemfile
```

```ruby
source 'https://rubygems.org'
gem 'nokogiri'
gem 'rack', '~>1.1'
gem 'rspec', :require => 'spec'
```

```bash
bundle install
```

====

## <i class="br br-ruby"></i> BDD com rspec

http://rspec.info

http://betterspecs.org

```ruby
describe Calculator do
  let(:calc) { Calculator.new() }

  describe '#sum' do
    subject { calc.sum 2, 8 }

    it 'sums two numbers' do
      is_expected.to eq 10
    end
  end
end
```

----

## <i class="br br-rails"></i> Convenções bem definidas

Ruby on Rails segue a filosofia _Convention over configuration_

- Reduz o número de decisões do desenvolvedor
- Fácil de obter ajuda da comunidade

```ruby
class Project < ApplicationRecord
  belongs_to :account
  has_many :participants, class_name: ‘Person’
  validates_presence_of :name
end
```

====

## <i class="br br-rails"></i> Setup rápido

```bash
gem install rails
rails new blog
cd blog
bin/rails server
```

====

## <i class="br br-rails"></i> Asset Pipeline

Dispensa/substitui Grunt, Gulp, etc.

- CSS, SASS
- Javascript, CoffeeScript
- Compila, concatena, minifica

----

## <i class="fa fa-check"></i> O que Ruby on Rails resolve?

- Aplicações web diversas
    + e-commerce
    + portais / redes sociais
    + gerenciamento de conteúdo
- Criação rápida
    + "favorito das _startups_"
- Deploy facilitado

====

## <i class="fa fa-ban"></i> Onde não usar?

- Sistemas altamente distribuídos / APIs
- Aplicações Desktop

====

## <i class="br br-ruby"></i> Outras coisas Ruby

- Sinatra (http://www.sinatrarb.com)
    + para APIs
- Jekyll (https://jekyllrb.com/)
    + sites estáticos, blogs, GitHub pages
- Ruby Motion (http://www.rubymotion.com/)
    + cross-plataform Mobile apps
- Chef (https://www.chef.io/chef/)
    + DevOps
- Vagrant (https://www.vagrantup.com)
    + infra, ambientes de desenvolvimento

====

## <i class="fa fa-calendar"></i> Eventos

- <i class="br br-ruby"></i> RubyConf (http://rubyconf.com.br)
- <i class="fa fa-heart"></i> Rails Girls (http://railsgirls.com)
- **GURU** - Grupo de usuários Ruby

----
<!-- .slide: data-background="url(img/feanor.jpg)" data-background-size="contain" data-background-repeat="no-repeat" data-background-position="right" -->

# Dúvidas? <!-- .element: class="pull-left" -->

&nbsp;

Note:
Image credits: Fëanor, por Fabiana Amaral
