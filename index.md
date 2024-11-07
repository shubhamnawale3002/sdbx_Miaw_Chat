<script type='text/javascript' src='https://service.force.com/embeddedservice/5.0/esw.min.js'></script>
<script type='text/javascript'>
	function initEmbeddedMessaging() {
		try {
			embeddedservice_bootstrap.settings.language = 'en_US'; // For example, enter 'en' or 'en-US'
			embeddedservice_bootstrap.settings.omitSandbox = true;
			localStorage.setItem('embeddedMessagingLanguage', embeddedservice_bootstrap.settings.language);
			embeddedservice_bootstrap.init(
				'00DTH000000t9kD',
				'Sonim_Chat_Support',
				'https://mtechmdm--voicebox.sandbox.my.site.com/ESWSonimChatSupport1723196645426',
				{
					scrt2URL: 'https://mtechmdm--voicebox.sandbox.my.salesforce-scrt.com'
				}
			);
		} catch (err) {
			console.error('Error loading Embedded Messaging: ', err);
		}
	};
</script>
<script type='text/javascript' src='https://mtechmdm--voicebox.sandbox.my.site.com/ESWSonimChatSupport1723196645426/assets/js/bootstrap.min.js' onload='initEmbeddedMessaging()'></script>
