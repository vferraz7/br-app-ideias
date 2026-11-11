# Charity Finder

**Nível:** 2-Intermediário

Com o app Charity Finder você não apenas vai aprimorar suas habilidades
de Desenvolvedor Web, mas também terá a oportunidade de ver como pode
fazer o bem. O objetivo deste app é utilizar a API da organização
[Global Giving](https://www.globalgiving.org/) para fornecer aos seus
usuários uma lista de ONGs globais que podem ser buscadas para encontrar
uma organização que corresponda aos seus interesses filantrópicos.

### Restrições

- Como o app pede ao usuário para escolher and contribuir para uma causa
  beneficente é importante que a apresentação da informação seja clara
  and concisa.
  Igualmente importante é a necessidade de que a UI/UX seja polida and
  envolvente para usar.

  Embora isso seja verdade para todos os apps, é ainda mais o caso
  aqui já que cada usuário que abandona o site representa a perda de
  uma oportunidade de fazer o bem (veja ['What is Web Site Conversion?](#useful-links-and-resources)) abaixo.

## Histórias de Usuário

-   [ ] O usuário pode ver um cabeçalho da página contendo o nome da
    aplicação.
-   [ ] O usuário pode ver uma visão geral do propósito do app em formato
    de 'página de apresentação'.
-   [ ] O usuário pode ver uma área de busca contendo um conjunto de caixas
    de seleção que permitem ao usuário especificar critérios de busca para
    organizações beneficentes incluindo:
    - Nome da organização
    - País de origem da organização
    - Países onde a organização atua
-   [ ] O usuário pode ver um botão 'Buscar'
-   [ ] O usuário pode clicar no botão 'Buscar' para exibir cartões de
    informação para as organizações correspondentes em uma área de
    resultados de busca.
-   [ ] O usuário pode ver cartões de informação da organização na área
    de resultados de busca contendo:
    - ID
    - Nome
    - Endereço
    - Logo
-   [ ] O usuário pode clicar no logotipo no cartão de informação da
    organização para abrir uma nova janela para a página inicial daquela
    organização.
-   [ ] O usuário pode ver um rodapé da página com links para seu GitHub
    and contas de redes sociais incluindo ícones de redes sociais (como
    o ícone do Twitter).

## Funcionalidades Bônus

-   [ ] O usuário pode ver uma caixa de busca para temas que a ONG foca.
-   [ ] O usuário pode selecionar múltiplas opções nas caixas de busca.
-   [ ] O usuário pode ver um link de projeto (ex: 'PROJETO') no cartão
    de informação da organização.
-   [ ] O usuário pode clicar no link do projeto para exibir uma página
    com informações descrevendo o projeto da Global Giving com o qual
    a organização está associada.
    Dica: examine a estrutura do JSON retornado pela API para entender
    a relação entre projetos and organizações.

## Links e Recursos Úteis

- [What is Web Site Conversion?](https://www.marketing91.com/what-is-website-conversion/)
- [Global Giving API](https://www.globalgiving.org/api/)
- Exemplo XML para um projeto retornado pela API:
```
<?xml version="1.0" encoding="UTF-8" standalone="yes"?>
<projects numberFound="26842">
    <hasNext>true</hasNext>
    <nextProjectId>367</nextProjectId>
    <project>
        <active>false</active>
        <activities>To fund the training of health professionals including nurses, psychologists, and social workers, and buy medicine and equipment.</activities>
        <additionalDocumentation>https://www.globalgiving.org/pfil/359/projdoc.doc</additionalDocumentation>
        <approvedDate>2004-06-01T12:43:27-04:00</approvedDate>
        <contactAddress>28 Pine Street</contactAddress>
        <contactCity>Mechanic Falls</contactCity>
        <contactCountry>United States</contactCountry>
        <contactPostal>04256</contactPostal>
        <contactState>Maine</contactState>
        <contactUrl>http://groups.yahoo.com/group/FOCUSonCambodia</contactUrl>
        <country>Cambodia</country>
        <funding>8239.33</funding>
        <goal>55000.00</goal>
        <id>359</id>
        <image id="0">
            <imagelink size="small">
                <url>https://www.globalgiving.org/pfil/359/pict_grid1.jpg</url>
            </imagelink>
            <imagelink size="thumbnail">
                <url>https://www.globalgiving.org/pfil/359/pict_thumbnail.jpg</url>
            </imagelink>
            <imagelink size="medium">
                <url>https://www.globalgiving.org/pfil/359/pict_med.jpg</url>
            </imagelink>
            <imagelink size="large">
                <url>https://www.globalgiving.org/pfil/359/pict_grid7.jpg</url>
            </imagelink>
            <imagelink size="extraLarge">
                <url>https://www.globalgiving.org/pfil/359/pict_large.jpg</url>
            </imagelink>
            <imagelink size="original">
                <url>https://www.globalgiving.org/pfil/359/pict_original.jpg</url>
            </imagelink>
            <title>Improving the Health of Children in Cambodia</title>
        </image>
        <imageGallerySize>1</imageGallerySize>
        <imageLink>https://www.globalgiving.org/pfil/359/pict.jpg</imageLink>
        <iso3166CountryCode>KH</iso3166CountryCode>
        <longTermImpact>This project will help improve the mental and physical health of orphaned children in Cambodia.  This project will also ensure the sustainability of the Nutrition Center in Child Mental Health Center.</longTermImpact>
        <need>Our beneficiaries will be orphaned children suffering from AIDS/HIV and other diseases and children with mental health problems whose parents do not know how to cope because they were deprived of family experiences by the forced separations of the Pol Pot regime. At the Nutrition Center in Phnom Penh, we will help urban orphans from brothels and hospitals that have abandoned them. At the Child Mental Health Center, we will help families, largely the working poor, from all over Cambodia.</need>
        <numberOfDonations>102</numberOfDonations>
        <organization>
            <activeProjects>0</activeProjects>
            <addressLine1>1062 Lewiston Road</addressLine1>
            <addressLine2></addressLine2>
            <bridgeId>5824171103</bridgeId>
            <city>New Gloucester</city>
            <countries>
                <country>
                    <iso3166CountryCode>KH</iso3166CountryCode>
                    <name>Cambodia</name>
                </country>
            </countries>
            <country>United States</country>
            <id>10</id>
            <iso3166CountryCode>US</iso3166CountryCode>
            <mission>The mission of FOCUS is to pursue humanitarian programs that include medical aid, school construction and supplies, distribution of rice and rice seeds, road improvements, agricultural improvements, fish farms, basic housing, hospital restoration, school scholarships, and loans for infrastructure improvements. We want to help disadvantaged youth and their families, if they have any, in a country where the infrastructure is still weak due to Khmer Rouge depredations.</mission>
            <name>Friends of Cambodia in the U.S.  (FOCUS)</name>
            <postal>4260</postal>
            <state>Maine</state>
            <themes>
                <theme>
                    <id>health</id>
                    <name>Health</name>
                </theme>
            </themes>
            <totalProjects>2</totalProjects>
            <url></url>
        </organization>
        <progressReportLink>https://www.globalgiving.org/projects/educating-children-of-cambodia/updates/</progressReportLink>
        <projectLink>https://www.globalgiving.org/projects/educating-children-of-cambodia/</projectLink>
        <region>Asia and Oceania</region>
        <remaining>46760.67</remaining>
        <status>funded</status>
        <summary>To help abandoned children, many afflicted with HIV/AIDS, and children with mental health problems. We want to address lack of food, medicine and staff training.</summary>
        <themeName>Health</themeName>
        <title>Improving the Health of Children in Cambodia</title>
        <type>project</type>
    </project>
</projects>
```

## Projetos de Exemplo

[Playing with card layout](https://codepen.io/bradjdouglas/pen/xOZJRz)