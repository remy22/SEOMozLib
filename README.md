SEOMozLib
=========

C# wrapper for the SEOmoz API

Example
=========

var moz = new Mozscape()
{
	MozAccessId = "member-6cf73fg9d8",
	MozSecretKey = "447b8340513d46ebcf58efgf3d2deaf5",
	MozApiType = MozAPI.URL_METRICS
};

var url = moz.CreateMozAPIUrl("pixelmedia.com/", MozAPI.URL_METRICS, 1);

var results = moz.GetRawResults(url);