<script type='text/javascript'>
	function initEmbeddedMessaging() {
		console.log('Initializing Embedded Messaging...'); // Log when the function starts

		try {
			console.log('Setting language for embedded service:', 'en_US');
			embeddedservice_bootstrap.settings.language = 'en_US'; // For example, enter 'en' or 'en-US'
			console.log('Language set successfully.');

			console.log('Preparing to initialize embedded service with parameters:', {
				orgId: '00D5j00000DCDP7',
				siteName: 'Sonim',
				siteURL: 'https://shubhamdeveloper-dev-ed.develop.my.site.com/ESWSonim1743513113880',
				scrt2URL: 'https://shubhamdeveloper-dev-ed.develop.my.salesforce-scrt.com'
			});

			// Initialization
			console.log('Calling embeddedservice_bootstrap.init...');
			embeddedservice_bootstrap.init(
				'00D5j00000DCDP7',
				'Sonim',
				'https://shubhamdeveloper-dev-ed.develop.my.site.com/ESWSonim1743513113880',
				{
					scrt2URL: 'https://shubhamdeveloper-dev-ed.develop.my.salesforce-scrt.com'
				}
			);
			console.log('embeddedservice_bootstrap.init called successfully.');

			console.log('Checking if embedded service is initialized correctly...');
			if (embeddedservice_bootstrap && embeddedservice_bootstrap.settings.language === 'en_US') {
				console.log('Embedded Messaging initialized successfully with language:', embeddedservice_bootstrap.settings.language);
			} else {
				console.warn('Embedded Messaging initialized, but language setting may not be applied correctly.');
			}

		} catch (err) {
			console.error('Error loading Embedded Messaging:', err);
			console.trace('Stack trace for error:');
		}
	};
</script>

<script type='text/javascript' src='https://shubhamdeveloper-dev-ed.develop.my.site.com/ESWSonim1743513113880/assets/js/bootstrap.min.js' onload='initEmbeddedMessaging()'></script>
