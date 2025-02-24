<script type='text/javascript' src='https://service.force.com/embeddedservice/5.0/esw.min.js'></script>
<script type='text/javascript'>
	function initEmbeddedMessaging() {
		try {
			embeddedservice_bootstrap.settings.language = 'en_US'; // For example, enter 'en' or 'en-US'
			embeddedservice_bootstrap.settings.omitSandbox = true;
			embeddedservice_bootstrap.init(
				'00DHr00000IGvvi',
				'Agentforce_Service_Agent_ESD',
				'https://in1738905200956.my.site.com/ESWAgentforceServiceAge1739166687729',
				{
					scrt2URL: 'https://in1738905200956.my.salesforce-scrt.com'
				}
			);
		} catch (err) {
			console.error('Error loading Embedded Messaging: ', err);
		}
	};
</script>
<script type='text/javascript' src='https://in1738905200956.my.site.com/ESWAgentforceServiceAge1739166687729/assets/js/bootstrap.min.js' onload='initEmbeddedMessaging()'></script>

