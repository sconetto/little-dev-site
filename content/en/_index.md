---
title: 'Home'
type: landing

sections:
  - block: hero
    content:
      title: Little Development Technology
      text: |
        <b>Make your business great, leave the little developments to us!</b><br><br>
        Technology and consultancy solutions to boost your business.
        We transform ideas into custom digital solutions.
      primary_action:
        text: Contact Us
        url: /#contact
        icon: chat-bubble-left-right
        style: gradient
      secondary_action:
        text: Our Services
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
            Countries  
            served
        - statistic: "2+"
          description: |
            Years in  
            the market
        - statistic: "10+"
          description: |
            Years of team  
            experience
        - statistic: "100%"
          description: |
            On-time delivery,
            end-to-end
    design:
      layout: minimal
      numbers_gradient: true
      css_class: "bg-white dark:bg-gray-900"
      spacing:
        padding: ["3rem", 0, "3rem", 0]

  - block: steps
    id: how-it-works
    content:
      subtitle: How we work
      title: Our process for projects
      text: From initial idea to delivery, made simple with transparent and efficient processes.
      items:
        - title: Understand your vision
          text: We start with your reality. We map your needs, goals, and challenges to propose the best solution.
          icon: chat-bubble-left-right
        - title: Plan and design
          text: We create a detailed plan with timeline, technologies, and architecture.<br/>You know exactly what to expect, no surprises!
          icon: clipboard-document-list
        - title: Develop with excellence
          text: Our team delivers complete and quality solutions, with agile methodologies, automated tests, and continuous reviews.
          icon: code-bracket
        - title: Deliver and care
          text: We launch your solution and provide ongoing support to ensure everything runs perfectly, <b>ALWAYS!</b>
          icon: rocket-launch
    design:
      layout: horizontal
      marker_style: icon
      connector: none

  - block: features
    id: services
    content:
      subtitle: What we do
      title: Our services and solutions
      text: We offer complete technology and consultancy solutions to help your business grow.
      items:
        - name: System Development
          icon: code-bracket
          description: Services, automations, websites, landing pages, portals, and complete applications using the best technologies available.
        - name: IT Consulting
          icon: light-bulb
          description: Specialized technical advisory to help your business make the best technology decisions.
        - name: Digital Transformation
          icon: presentation-chart-bar
          description: Strategy consulting and implementation of digital processes for your company.
        - name: APIs & Integrations
          icon: server-stack
          description: Robust API development and system integrations to automate your business processes.
        - name: Support & Maintenance
          icon: wrench-screwdriver
          description: Ongoing technical support and system maintenance to keep your business running smoothly.
        - name: Cloud & DevOps
          icon: cloud
          description: Cloud migration, infrastructure as code, and CI/CD pipelines for faster deliveries.
    design:
      layout: bento
      css_class: "bg-gray-50 dark:bg-gray-900/50"

  - block: cta-image-paragraph
    id: about
    content:
      items:
        - title: About Us
          subtitle: Our story
          text: |
            Little Development Technology ― <i>LD Tech</i> ― was born from a passion
            for technology and the belief that well-developed solutions transform
            businesses. We are a team dedicated to delivering excellence in every
            project, focusing on quality, value, and customer satisfaction.
            <br/><br/>
            Our vision is straightforward: you focus on making your company the best
            in the market while we help you with digital solutions.
            <br/><br/>
            <b>Get in touch and discover how we can help your business grow.</b>
          feature_icon: check
          features:
            - "Specialized and experienced team"
            - "Tailored solutions for your business"
            - "Dedicated and ongoing support"
            - "Agile development methodologies"
          button:
            text: Contact Us
            url: /#contact
    design:
      css_class: "bg-white dark:bg-gray-900"

  - block: faq
    id: faq
    content:
      title: Frequently Asked Questions
      subtitle: Everything you need to know before getting started.
      items:
        - question: How long does it take to develop a system?
          answer: |
            It depends on the project's complexity. Simpler systems can take a few weeks to a month, while more complex applications can take 2 to 6 months. During the initial consultation, we provide a detailed project timeline and only proceed with your approval.
        - question: What technologies do you use?
          answer: |
            We work with the best technologies in the market, including React, Next.js, Flutter, Node.js, Python, Go, and more. The technology choice depends on your project's specific needs.
        - question: Do you offer post-delivery support?
          answer: |
            Yes! We offer ongoing support and maintenance plans to keep your system updated, secure, and running smoothly.
        - question: How does the quotation process work?
          answer: |
            After an initial conversation to understand your project, we prepare a detailed proposal with scope, timeline, and investment. No commitment required.
        - question: Do you serve companies of all sizes?
          answer: |
            Yes! We serve from early-stage startups to large enterprises. Every project is handled with the same dedication and excellence.
        - question: Do you handle legacy system migration?
          answer: |
            Yes, we have experience modernizing legacy systems, migrating to current technologies without disrupting your operations.
    design:
      css_class: "bg-gray-50 dark:bg-gray-900/50"

  - block: cta-image-paragraph
    id: contact
    content:
      items:
        - title: Get in Touch
          text: |
            Have a project in mind?<br/>We would love to hear about it.
            <br/><br/>
            <b>Email:</b> <a href="mailto:contact@littledevelopment.tech"><i>contact@littledevelopment.tech</i></a></br>
            <b>WhatsApp</b> <a href="https://wa.me/5561920033989" target="_blank"><i>+55 (61) 92003-3989</i></a></br>
            <br/>
            Send us a message and we will get back to you within 24 hours.
          feature_icon: check
          features:
            - "Free no-obligation consultation"
            - "Transparent and detailed quote"
            - "Personalized service"
          button:
            text: Contact us on WhatsApp
            url: https://wa.me/5561920033989

  - block: cta-card
    content:
      title: Ready to turn your idea into reality?
      text: Get in touch today and discover how Little Development can help your business grow.
      button:
        text: Contact Us
        url: /#contact
    design:
      card:
        css_class: "bg-gradient-to-br from-primary-500 via-primary-600 to-secondary-600 text-white shadow-2xl"
---
