# poetry-functions
##These were my very first attempts at functions that generate poems. The functions aren't 
#sophisticated, but the poems come out really nice.

import random

def r(L):
	return random.sample(L,1)[0]

def poem():
	subjects=['happiness','sunshine','unicorn','moonlight','magic','he','she','they','eyes']
	objects=['her','love','baby','majesty','him','affection']
	transitives=['held','loved','belonged to', 'believed', 'cursed','kissed','imagined','saw','sparkled']
	intransitives=['died','wept','fainted']
	adverbs=['slowly','softly','lovingly','faintly','perfectly']
	adjectives=['her','their','magic','dirty','perfect','crystal','equine','soft','tangled','dewy']
	title=str.upper(r(adjectives)+' '+r(objects))
	a=r(adverbs)+' '+r(subjects)+' '+r(intransitives)
	print(title,'\n ','\n ',r(subjects),r(transitives),r(objects),';\n ',a,';\n ',r(subjects),'was',r(adverbs),r(adjectives),';\n ', r(adverbs),r(adverbs),r(adverbs),';\n ',r(subjects),r(adverbs),r(transitives),r(adjectives),r(objects),';\n ',a,'.')


def poem2():
	subjects=['happiness','sunshine','unicorn','moonlight','magic','he','she','they','eyes']
	objects=['her','love','baby','majesty','him','affection','curls']
	transitives=['held','loved','belonged to', 'believed', 'cursed','kissed','imagined','saw','sparkled','awakened']
	intransitives=['died','wept','fainted','hissed']
	adverbs=['slowly','softly','lovingly','faintly','perfectly']
	adjectives=['her','their','magic','dirty','perfect','crystal','equine','soft','tangled','dewy','mossy','green','sweet','rotten','dirt-smelling']
	title=str.upper(r(adjectives)+' '+r(objects))
	a=r(adverbs)+' '+r(subjects)+' '+r(intransitives)
	print(title,'\n ','\n ',r(subjects),r(transitives),r(objects),';\n ',a,';\n ',r(subjects),'was',r(adverbs),r(adjectives),';\n ', r(adverbs),r(adverbs),r(adverbs),';\n ',r(subjects),r(adverbs),r(transitives),r(adjectives),r(objects),';\n ',r(subjects),r(intransitives),';\n ',a,'.')
