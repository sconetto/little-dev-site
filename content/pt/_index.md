---
title: 'Home'
type: landing

sections:
  - block: hero
    content:
      title: Little Development Tecnologia
      text: |
        <b>Faça seu negócio decolar, deixe os pequenos desenvolvimentos conosco!</b><br><br>
        Soluções em tecnologia e consultoria para impulsionar o seu negócio.
        Transformamos ideias em soluções digitais sob medida.
      primary_action:
        text: Fale Conosco
        url: /#contact
        icon: chat-bubble-left-right
        style: gradient
      secondary_action:
        text: Nossos Serviços
        url: /#services
        icon: code-bracket
        style: ghost
    design:
      spacing:
        padding: [0, 0, 0, 0]
        margin: [0, 0, 0, 0]
      background:
        text_color_light: true
        color: "#0a0e27"
        gradient:
          type: radial
          start: "rgba(59,130,246,0.35)"
          end: "transparent"
          position: "50% -10%"
          shape: ellipse
          size: "80% 80%"

  - block: stats
    content:
      items:
        - statistic: "4+"
          description: |
            Países  
            atendidos
        - statistic: "2+"
          description: |
            Anos de  
            mercado
        - statistic: "10+"
          description: |
            Anos de experiência  
            da equipe
        - statistic: "100%"
          description: |
            Entrega no prazo,
            do início ao fim
    design:
      layout: minimal
      numbers_gradient: true
      css_class: "bg-white dark:bg-gray-900"
      spacing:
        padding: ["3rem", 0, "3rem", 0]

  - block: steps
    id: how-it-works
    content:
      subtitle: Como trabalhamos
      title: Nosso processo em projetos
      text: Uma ideia inicial até a entrega de maneira simples, com processos transparentes e eficientes.
      items:
        - title: Entendemos sua visão
          text: Começamos com a sua realidade. Mapeamos suas necessidades, objetivos e desafios para propor a melhor solução.
          icon: chat-bubble-left-right
        - title: Planejamos e projetamos
          text: Criamos um plano detalhado com cronograma, tecnologias e arquitetura.<br/>Você sabe exatamente o que esperar, sem surpresas!
          icon: clipboard-document-list
        - title: Desenvolvemos com excelência
          text: Nosso time entrega soluções completas e de qualidade, com metodologias ágeis, testes automatizados e revisões contínuas.
          icon: code-bracket
        - title: Entregamos e cuidamos
          text: Lançamos sua solução e oferecemos suporte contínuo para garantir que tudo funcione perfeitamente, <b>SEMPRE!</b>
          icon: rocket-launch
    design:
      layout: horizontal
      marker_style: icon
      connector: none

  - block: features
    id: services
    content:
      subtitle: O que fazemos
      title: Nossos serviços e soluções
      text: Oferecemos soluções completas em tecnologia e consultoria para ajudar sua empresa a crescer.
      items:
        - name: Desenvolvimento de sistemas
          icon: code-bracket
          description: Serviços, automatizações, sites, landing pages, portais e diversas aplicações completas com as melhores tecnologias do mercado.
        - name: Consultoria em TI
          icon: light-bulb
          description: Assessoria técnica especializada para ajudar sua empresa a tomar as melhores decisões em tecnologia.
        - name: Transformação digital
          icon: presentation-chart-bar
          description: Consultoria em estrategia e implementação de processos digitais para sua empresa.
        - name: APIs e Integrações
          icon: server-stack
          description: Desenvolvimento de APIs robustas e integração entre sistemas para automatizar seus processos.
        - name: Suporte e Manutenção
          icon: wrench-screwdriver
          description: Suporte técnico contínuo e manutenção de sistemas para garantir o funcionamento do seu negócio.
        - name: Cloud e DevOps
          icon: cloud
          description: Migração para nuvem, infraestrutura como código e pipelines de CI/CD para entregas mais rápidas.
    design:
      layout: bento
      css_class: "bg-gray-50 dark:bg-gray-900/50"

  - block: cta-image-paragraph
    id: about
    content:
      items:
        - title: Sobre Nós
          subtitle: A nossa história
          text: |
            A Little Development Tecnologia ― <i>LD Tech</i> ― nasceu da paixão por tecnologia e da certeza de que
            soluções bem desenvolvidas transformam negócios. Somos uma equipe dedicada
            a entregar excelência em cada projeto, com foco em qualidade, valor e
            satisfação do cliente.
            <br/><br/>
            Nossa visão é direta, você se preocupa em tornar sua empresa a melhor no mercado
            enquanto nos te ajudamos com soluções digitais.
            <br/><br/>
            <b>Entre em contato e descubra como podemos ajudar o seu negócio a crescer.</b>
          feature_icon: check
          features:
            - "Equipe especializada e experiente"
            - "Soluções sob medida para seu negócio"
            - "Suporte dedicado e contínuo"
            - "Metodologias ágeis de desenvolvimento"
          button:
            text: Fale Conosco
            url: /#contact
    design:
      css_class: "bg-white dark:bg-gray-900"

  - block: faq
    id: faq
    content:
      title: Perguntas Frequentes
      subtitle: Tudo que você precisa saber antes de começar.
      items:
        - question: Quanto tempo leva para desenvolver um sistema?
          answer: |
            Depende da complexidade do projeto. Um sistemas mais simples podem levar de semanas a um mês, enquanto aplicações mais complexas podem levar de 2 a 6 meses. Durante a consultoria inicial, fornecemos um cronograma detalhado do projeto e só damos prosseguimento com a sua aprovação.
        - question: Quais tecnologias vocês utilizam?
          answer: |
            Trabalhamos com as melhores tecnologias do mercado, incluindo React, Next.js, Flutter, Node.js, Python, Go, entre outras. A escolha da tecnologia depende das necessidades específicas do seu projeto.
        - question: Vocês oferecem suporte após a entrega?
          answer: |
            Sim! Oferecemos planos de suporte e manutenção contínua para garantir que seu sistema permaneça atualizado, seguro e funcionando perfeitamente.
        - question: Como funciona o processo de orçamento?
          answer: |
            Após uma conversa inicial para entender seu projeto, preparamos uma proposta detalhada com escopo, cronograma e investimento. Sem compromisso.
        - question: Vocês atendem empresas de qualquer porte?
          answer: |
            Sim! Atendemos desde startups em estágio inicial até grandes empresas. Cada projeto é tratado com a mesma dedicação e excelência.
        - question: Fazem migração de sistemas legados?
          answer: |
            Sim, temos experiência em modernizar sistemas legados, migrando para tecnologias atuais sem interromper suas operações.
    design:
      css_class: "bg-gray-50 dark:bg-gray-900/50"

  - block: cta-image-paragraph
    id: contact
    content:
      items:
        - title: Entre em Contato
          text: |
            Tem um projeto em mente?<br/>Adoraríamos ouvir sobre ele.
            <br/><br/>
            <b>Email:</b> <a href="mailto:contact@littledevelopment.tech"><i>contact@littledevelopment.tech</i></a><br/>
            <b>WhatsApp</b> <a href="https://wa.me/5561920033989" target="_blank"><i>+55 (61) 92003-3989</i></a><br/>
            <br/>
            Mande uma mensagem e retornaremos em até 24 horas.
          feature_icon: check
          features:
            - "Uma conversa para consultar seu projeto sem custo e sem compromisso"
            - "Orçamento transparente e detalhado"
            - "Atendimento personalizado"
          button:
            text: Fale Conosco no WhatsApp
            url: https://wa.me/5561920033989

  - block: cta-card
    content:
      title: Pronto para transformar sua ideia em realidade?
      text: Entre em contato hoje mesmo e descubra como a Little Development pode ajudar seu negócio a crescer.
      button:
        text: Fale Conosco
        url: /#contact
    design:
      card:
        css_class: "bg-gradient-to-br from-primary-500 via-primary-600 to-secondary-600 text-white shadow-2xl"
---
