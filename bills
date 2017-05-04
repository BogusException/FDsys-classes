   /* 
    Licensed under the Apache License, Version 2.0
    
    http://www.apache.org/licenses/LICENSE-2.0
    */
using System;
using System.Xml.Serialization;
using System.Collections.Generic;

namespace bills.hconres
{
	[XmlRoot(ElementName="action")]
	public class Action {
		[XmlElement(ElementName="action-date")]
		public Actiondate Actiondate { get; set; }
		[XmlElement(ElementName="action-desc")]
		public Actiondesc Actiondesc { get; set; }
		[XmlAttribute(AttributeName="display")]
		public string Display { get; set; }
	}

	[XmlRoot(ElementName="action-date")]
	public class Actiondate {
		[XmlAttribute(AttributeName="date")]
		public string Date { get; set; }
		[XmlText]
		public string Text { get; set; }
	}

	[XmlRoot(ElementName="action-desc")]
	public class Actiondesc {
		[XmlElement(ElementName="committee-name")]
		public Committeename Committeename { get; set; }
		[XmlElement(ElementName="cosponsor")]
		public List<Cosponsor> Cosponsor { get; set; }
		[XmlElement(ElementName="sponsor")]
		public Sponsor Sponsor { get; set; }
	}

	[XmlRoot(ElementName="committee-name")]
	public class Committeename {
		[XmlAttribute(AttributeName="committee-id")]
		public string Committeeid { get; set; }
		[XmlText]
		public string Text { get; set; }
	}

	[XmlRoot(ElementName="congress")]
	public class Congress {
		[XmlAttribute(AttributeName="display")]
		public string Display { get; set; }
		[XmlText]
		public string Text { get; set; }
	}

	[XmlRoot(ElementName="cosponsor")]
	public class Cosponsor {
		[XmlAttribute(AttributeName="name-id")]
		public string Nameid { get; set; }
		[XmlText]
		public string Text { get; set; }
	}

	[XmlRoot(ElementName="distribution-code")]
	public class Distributioncode {
		[XmlAttribute(AttributeName="display")]
		public string Display { get; set; }
		[XmlText]
		public string Text { get; set; }
	}

	[XmlRoot(ElementName="dublinCore")]
	public class DublinCore {
		[XmlElement(ElementName="date", Namespace="http://purl.org/dc/elements/1.1/")]
		public string Date { get; set; }
		[XmlElement(ElementName="format", Namespace="http://purl.org/dc/elements/1.1/")]
		public string Format { get; set; }
		[XmlElement(ElementName="language", Namespace="http://purl.org/dc/elements/1.1/")]
		public string Language { get; set; }
		[XmlElement(ElementName="publisher", Namespace="http://purl.org/dc/elements/1.1/")]
		public string Publisher { get; set; }
		[XmlElement(ElementName="rights", Namespace="http://purl.org/dc/elements/1.1/")]
		public string Rights { get; set; }
		[XmlElement(ElementName="title", Namespace="http://purl.org/dc/elements/1.1/")]
		public string Title { get; set; }
	}

	[XmlRoot(ElementName="form")]
	public class Form {
		[XmlElement(ElementName="action")]
		public Action Action { get; set; }
		[XmlElement(ElementName="congress")]
		public Congress Congress { get; set; }
		[XmlElement(ElementName="current-chamber")]
		public string Currentchamber { get; set; }
		[XmlElement(ElementName="distribution-code")]
		public Distributioncode Distributioncode { get; set; }
		[XmlElement(ElementName="legis-num")]
		public Legisnum Legisnum { get; set; }
		[XmlElement(ElementName="legis-type")]
		public string Legistype { get; set; }
		[XmlElement(ElementName="official-title")]
		public Officialtitle Officialtitle { get; set; }
		[XmlElement(ElementName="session")]
		public Session Session { get; set; }
	}

	[XmlRoot(ElementName="legis-num")]
	public class Legisnum {
		[XmlAttribute(AttributeName="display")]
		public string Display { get; set; }
		[XmlText]
		public string Text { get; set; }
	}

	[XmlRoot(ElementName="metadata")]
	public class Metadata {
		[XmlAttribute(AttributeName="dc", Namespace="http://www.w3.org/2000/xmlns/")]
		public string Dc { get; set; }
		[XmlElement(ElementName="dublinCore")]
		public DublinCore DublinCore { get; set; }
	}

	[XmlRoot(ElementName="official-title")]
	public class Officialtitle {
		[XmlAttribute(AttributeName="display")]
		public string Display { get; set; }
		[XmlText]
		public string Text { get; set; }
	}

	[XmlRoot(ElementName="paragraph")]
	public class Paragraph {
		[XmlElement(ElementName="enum")]
		public string Enum { get; set; }
		[XmlAttribute(AttributeName="id")]
		public string Id { get; set; }
		[XmlElement(ElementName="text")]
		public Text Text { get; set; }
	}

	[XmlRoot(ElementName="preamble")]
	public class Preamble {
		[XmlElement(ElementName="whereas")]
		public List<Whereas> Whereas { get; set; }
	}

	[XmlRoot(ElementName="resolution")]
	public class Resolution {
		[XmlAttribute(AttributeName="dms-id")]
		public string Dmsid { get; set; }
		[XmlElement(ElementName="form")]
		public Form Form { get; set; }
		[XmlAttribute(AttributeName="key")]
		public string Key { get; set; }
		[XmlElement(ElementName="metadata")]
		public Metadata Metadata { get; set; }
		[XmlElement(ElementName="preamble")]
		public Preamble Preamble { get; set; }
		[XmlAttribute(AttributeName="public-private")]
		public string Publicprivate { get; set; }
		[XmlElement(ElementName="resolution-body")]
		public Resolutionbody Resolutionbody { get; set; }
		[XmlAttribute(AttributeName="resolution-stage")]
		public string Resolutionstage { get; set; }
		[XmlAttribute(AttributeName="resolution-type")]
		public string Resolutiontype { get; set; }
		[XmlAttribute(AttributeName="star-print")]
		public string Starprint { get; set; }
	}

	[XmlRoot(ElementName="resolution-body")]
	public class Resolutionbody {
		[XmlAttribute(AttributeName="id")]
		public string Id { get; set; }
		[XmlElement(ElementName="section")]
		public Section Section { get; set; }
		[XmlAttribute(AttributeName="style")]
		public string Style { get; set; }
	}

	[XmlRoot(ElementName="section")]
	public class Section {
		[XmlAttribute(AttributeName="display-inline")]
		public string Displayinline { get; set; }
		[XmlElement(ElementName="enum")]
		public string Enum { get; set; }
		[XmlAttribute(AttributeName="id")]
		public string Id { get; set; }
		[XmlAttribute(AttributeName="section-type")]
		public string Sectiontype { get; set; }
		[XmlElement(ElementName="text")]
		public string Text { get; set; }
	}

	[XmlRoot(ElementName="session")]
	public class Session {
		[XmlAttribute(AttributeName="display")]
		public string Display { get; set; }
		[XmlText]
		public string Text { get; set; }
	}

	[XmlRoot(ElementName="sponsor")]
	public class Sponsor {
		[XmlAttribute(AttributeName="name-id")]
		public string Nameid { get; set; }
		[XmlText]
		public string Text { get; set; }
	}

	[XmlRoot(ElementName="text")]
	public class Text {
		[XmlElement(ElementName="quote")]
		public List<string> Quote { get; set; }
	}

	[XmlRoot(ElementName="whereas")]
	public class Whereas {
		[XmlElement(ElementName="paragraph")]
		public List<Paragraph> Paragraph { get; set; }
		[XmlElement(ElementName="text")]
		public Text Text { get; set; }
	}

}
